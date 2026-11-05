# AWS CloudFormation – Implementando minha primeira Stack

## 1. Introdução

Este projeto foi desenvolvido como parte de um laboratório prático da Digital Innovation One (DIO), com o objetivo de aprender a utilizar o AWS CloudFormation para provisionar recursos na nuvem.

O AWS CloudFormation permite criar, configurar e gerenciar recursos da AWS por meio de arquivos de infraestrutura como código (Infrastructure as Code – IaC).

## 2. Objetivos

- Compreender o funcionamento do AWS CloudFormation.
- Criar uma primeira Stack na AWS.
- Utilizar templates no formato YAML.
- Automatizar a criação de recursos.
- Compreender o gerenciamento do ciclo de vida de uma infraestrutura.
- Documentar os conhecimentos adquiridos durante o laboratório.

## 3. O que é AWS CloudFormation?

O AWS CloudFormation é um serviço que permite modelar e provisionar recursos da AWS utilizando código.

Em vez de criar cada recurso manualmente pelo Console AWS, podemos definir toda a infraestrutura em um template e solicitar que o CloudFormation faça a implementação automaticamente.

Essa abordagem facilita a padronização, a replicação e a manutenção da infraestrutura.

## 4. Principais conceitos

### Stack

É um conjunto de recursos AWS gerenciados pelo CloudFormation como uma única unidade.

### Template

É o arquivo que descreve a infraestrutura que será criada. Pode ser escrito em YAML ou JSON.

### Resources

Define os recursos AWS que serão provisionados, como EC2, S3, RDS e VPC.

### Parameters

Permite receber valores externos para personalizar o template durante a criação da Stack.

### Outputs

Permite disponibilizar informações sobre os recursos criados, como IDs, nomes e endpoints.

### Change Sets

Permitem visualizar as alterações que serão realizadas em uma Stack antes de executá-las.

## 5. Implementação prática

Neste laboratório, a proposta é criar uma Stack utilizando AWS CloudFormation para provisionar um bucket Amazon S3.

O bucket será configurado com:

- Criptografia no servidor (SSE-S3).
- Versionamento de objetos habilitado.
- Bloqueio de acesso público.
- Identificação do projeto por tags.

O objetivo é demonstrar como o CloudFormation automatiza a criação e configuração de recursos.

## 6. Estrutura do projeto

```text
aws-cloudformation-lab/
│
├── README.md
│
├── templates/
│   └── infrastructure.yaml
│
└── images/
    ├── cloudformation-stack.png
    ├── stack-events.png
    └── resources-created.png
```

## 7. Benefícios do CloudFormation

- Automação da infraestrutura.
- Padronização dos ambientes.
- Facilidade para replicar recursos.
- Redução de erros manuais.
- Controle das alterações.
- Integração com outros serviços AWS.
- Possibilidade de versionar a infraestrutura utilizando Git.

## 8. Aprendizados

Durante este laboratório, o objetivo foi compreender como o AWS CloudFormation utiliza templates para automatizar o provisionamento de recursos.

A prática permite entender como o conceito de Infrastructure as Code facilita a administração de ambientes em nuvem, tornando a infraestrutura mais organizada, reproduzível e controlada.

## 9. Conclusão

O AWS CloudFormation é uma ferramenta importante para profissionais que trabalham com infraestrutura em nuvem.

A utilização de templates permite automatizar tarefas que normalmente seriam realizadas manualmente, facilitando a implantação e o gerenciamento de ambientes AWS.

## 10. Referências

- [Documentação oficial AWS CloudFormation](https://docs.aws.amazon.com/cloudformation/)
- [AWS CloudFormation User Guide](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)
- [Referência de recursos AWS](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html)

---

**Autor:** Anderson Otávio

**Plataforma:** Digital Innovation One (DIO)

**Serviço:** AWS CloudFormation

**Tecnologia:** Infrastructure as Code (IaC)
