---
layout: post
title: "Certificação HashiCorp Terraform Associate 003: Dicas, Experiências e Preparação"
author: orafaelferreiraa
categories: [Artigos, Certificação, HashiCorp Terraform Associate 003]
tags: [Artigos, Certificação, HashiCorp, Terraform]
---
# 

## Introdução

Fala galera! Tudo bom? Recentemente passei no exame **HashiCorp Certified: Terraform Associate (003)** e quero compartilhar com vocês um pouco sobre como foi a experiência, desde a estrutura da prova até as minhas dicas de estudo. Se você é um profissional de DevOps querendo se certificar em Terraform, este artigo é pra você!

Para quem não conhece, essa certificação Terraform Associate basicamente valida seus conhecimentos fundamentais sobre o Terraform e conceitos de Infraestrutura como Código (IaC).

[![HashiCorp Certified: Terraform Associate (003)](https://images.credly.com/size/118x118/images/ed4be915-68f8-428a-b332-40ded9084ee5/blob)](https://www.credly.com/badges/a2363246-1248-4028-a237-79b965fbcef3/public_url "HashiCorp Certified: Terraform Associate (003)")

## Sobre o Exame Terraform Associate

O Terraform Associate (versão 003) é uma certificação de nível "fundamental" da HashiCorp voltada para Terraform. É recomendada para engenheiros de infraestrutura/DevOps que atuam em operações, TI ou desenvolvimento e já conhecem os conceitos básicos do Terraform.

**Formato da prova:**
- Online, com supervisão (proctored)
- 57 questões de múltipla escolha
- Tempo: 1 hora (60 minutos)
- Idioma: Inglês
- Custo: cerca de US$70
- Validade: 2 anos

## Tópicos Principais do Exame

- **Infraestrutura como Código (IaC):** Saber o que é IaC e por que é vantajosa, destacando a consistência, automação e versionamento de infraestrutura.  
  - Exercício prático: [1-UnderstandInfrastructureasCode(IaC)concepts-BuildingVM](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/1-UnderstandInfrastructureasCode(IaC)concepts-BuildingVM)  
 
- **Propósito do Terraform em relação a outras ferramentas:** Entender os benefícios de ser multi-cloud e agnóstico ao provedor e o papel do arquivo de estado.  
  - Exercício prático: [2-UnderstandTerraformbasics](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/2-UnderstandTerraformbasics) 
- **Fundamentos do Terraform:** Dominar sintaxe HCL, blocos de recursos e dados, providers, variáveis e outputs.  
- **Uso do Terraform além do fluxo básico:** Conhecer comandos como `terraform import` para importar recursos, `terraform state` para inspecionar o estado e como habilitar logs de depuração.  
- **Módulos:** Saber encontrar módulos no registro público, usar módulos locais e remotos, versionar e entender o escopo de variáveis.
  - Exercício prático: [5-InteractwithTerraformmodules1](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/5-InteractwithTerraformmodules1) 
    - Exercício prático: [5-InteractwithTerraformmodules2](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/5-InteractwithTerraformmodules2)   
- **Fluxo de trabalho:** Gravar a sequência `write → plan → apply` (CAI NA PROVA) e também `validate`, `fmt` e `destroy`.  
- **Estado:** Entender backends locais e remotos, locking de estado, drifts e comandos como `terraform state mv`, bem como segredos no `tfstate`.  
- **Ler e modificar configurações:** Utilizar variáveis e outputs corretamente, proteger segredos, trabalhar com tipos complexos e funções HCL.  
  - Exercício prático: [8-Read,generate,ModifyConfiguration-Collections](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/8-Read%2Cgenerate%2CModifyConfiguration-Collections) 
    - Exercício prático: [8-Read,generate,ModifyConfiguration-Functions](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/8-Read%2Cgenerate%2CModifyConfiguration-Functions)  
    - Exercício prático: [8-Read,generate,ModifyConfiguration-Secrets](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate/8-Read%2Cgenerate%2CModifyConfiguration-Secrets) 
- **Conhecer o Terraform Cloud/Enterprise:** Ter noções das funcionalidades da oferta SaaS (state remoto, integração com VCS, políticas e colaboração).  
- **Workspaces:** Embora não apareça explicitamente no blueprint, várias questões NA PROVA abordam Workspaces. Saiba criar, listar, selecionar e remover workspaces e as diferenças em relação a usar backends distintos.

## Minha Preparação e Materiais de Estudo

- **Curso TFTEC:** 100% prático, com labs e simulado final. [Acesse aqui](https://tftec.curseduca.pro/m/c/terrafom-associate-1694628491755) 
- **Labs próprios:** Pratiquei com cloud Azure.  
- **GitHub pessoal:** Criei um [repositório](https://github.com/orafaelferreiraa/Terraform-Training-Projects/tree/main/Treinamento%20TFTEC%20Terrafom%20Associate) com todos os projetos que fiz nos labs.  
- **Curso Udemy – Terraform Associate Practice Exam (em inglês):** Excelente para testar conhecimentos com simulado realista. [Acesse aqui](https://www.udemy.com/course/terraform-associate-practice-exam/)

## Dicas para o Exame

- **Domine IaC na teoria:** O exame cobra definições e vantagens da IaC. Saiba explicar por que versionar infraestrutura como código aumenta a confiabilidade e como se diferencia de ferramentas de gerenciamento de configuração.  
- **Pratique todos os comandos:** Não fique só no trio `init/plan/apply`. Experimente `fmt`, `import`, `state list/show/mv`, `workspace`, `login/logout` e assim por diante.  
- **Estude o arquivo de estado:** Saiba que o `tfstate` é salvo localmente por padrão e pode ser movido para backends remotos. Entenda como funciona o locking, como lidar com drifts e quando usar `terraform state rm`.  
- **Módulos são fundamentais:** Crie e utilize módulos para entender entradas e saídas, escopo de variáveis, versionamento e fontes (local, registro ou repositório Git).  
- **Aprenda sobre Workspaces:** Domine os comandos `workspace new/list/select/show` e compreenda que cada workspace tem seu próprio arquivo de estado.  
- **Conheça o Terraform Cloud:** Mesmo que nunca tenha usado a versão SaaS, leia sobre suas vantagens: state remoto com bloqueio automático, integrações com Git, execução em equipe e políticas de governança.  
- **Gerencie o tempo na prova:** Sessenta minutos para 57 perguntas dá cerca de um minuto por questão. Marque a melhor opção e volte depois se necessário.  
- **Mantenha a calma:** Revise as opções com atenção, pois muitas vezes a diferença está em uma palavra (e em inglês). Antes de submeter, revise tudo.  
- **Transfira o aprendizado para o trabalho:** Refatore códigos reais com boas práticas. Aplicar o conteúdo no dia a dia reforça o aprendizado.

## Conclusão

Fazer a certificação Terraform Associate foi uma experiência valiosa. Além de receber o badge, consolidei conceitos essenciais de IaC e do Terraform que aplico diariamente. A prova reflete demandas do mundo real: ao estudar para ela, você aprimora seu domínio da ferramenta e se prepara melhor para projetos de nuvem e automação.

Recomendo a certificação para quem já utiliza Terraform. Ela formaliza o conhecimento e pode abrir portas — muitas vagas pedem familiaridade com Terraform, e ter a certificação ajuda a comprovar essa habilidade. Para quem pretende avançar, a HashiCorp oferece também o nível Professional, então a Associate pode ser só o começo.

![](https://stoblobcertificados011.blob.core.windows.net/imagens-blog/posts/2025-08-03-terraform-associate-artigo.png)

**Referências**:
- [HashiCorp Terraform Associate](https://developer.hashicorp.com/terraform/tutorials/certification-003/associate-review-003)