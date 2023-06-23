
# RESILIA DATA

---

##As entidades necessárias para criar o modelo são:

- Empresa
- Tecnologia
- Empresa_Tecnologia
- Colaborador

---
##Seus principais campos e tipos de dados são:

- **Empresa:**

        ID
        Nome
        Endereço
        Telefone
        Email

- **Tecnologia:**

        ID
        Nome
        Área de atuação

- **Empresa_Tecnologia:**

        ID_Empresa 
        ID_Tecnologia 

- **Colaborador:**

        ID 
        Nome 
        Cargo 
        ID_Empresa 
---
###Relacionamentos:

A tabela Empresa_Tecnologia representa a associação entre empresas e tecnologias, onde uma empresa pode utilizar várias tecnologias e uma tecnologia pode ser utilizada por várias empresas.
Já a tabela Colaborador possui uma relação de chave estrangeira com a tabela Empresa, indicando que um colaborador está associado a uma empresa específica.

---
###Simulando os registros:

__Empresa:__
ID: 1
Nome: Tecnology Exp
Endereço: Avenida Pres. Vargas, 615
Telefone: (21) 3462-5078
Email: tecnologyexp@tecnologyexp.com

ID: 2
Nome: Tech Science
Endereço: Avenida das Américas, 16546
Telefone: (21) 9859-5437
Email: techscience@techscience.com

__Tecnologia:__
ID: 1
Nome: Tecnologia X
Área: WebDev

ID: 2
Nome: Tecnologia Y
Área: Dados

__Empresa_Tecnologia:__
ID_Empresa: 1
ID_Tecnologia: 1

ID_Empresa: 2
ID_Tecnologia: 1

__Colaborador:__
ID: 1
Nome: Jonas Silva
Cargo: Desenvolvedor
ID_Empresa: 1

ID: 2
Nome: Josean Borgees
Cargo: Analista de Dados
ID_Empresa: 2


<div style="text-align: center;">
Sistema RESILIADATA
</div>
