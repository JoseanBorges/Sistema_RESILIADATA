
# RESILIA DATA
---

## As entidades necessárias para criar o modelo são:

- Empresa
- Tecnologia
- Empresa_Tecnologia
- Colaborador

---
## Seus principais campos e tipos de dados são:

- **Empresa:**

        ID - SERIAL(5)
        Nome - VARCHAR(150)
        Endereço - VARCHAR(220)
        Telefone - INT(15)
        Email - VARCHAR(50)

- **Tecnologia:**

        ID - SERIAL(5)
        Nome - VARCHAR(50)
        Área de atuação - VARCHAR(70)

- **Empresa_Tecnologia:**

        ID - SERIAL(5)
        ID_Empresa - SERIAL(5)
        ID_Tecnologia - SERIAL(5)

- **Colaborador:**

        ID - SERIAL(5)
        Nome - VARCHAR(150)
        CPF - INT(11)
        Endereço - VARCHAR(220)
        Telefone - INT(15)
        Email - VARCHAR(50)
        Cargo - VARCHAR(50)
        ID_Empresa - SERIAL(5)
---
### Relacionamentos:

Uma empresa pode ter várias tecnologias(relação 1,N).  

A tabela _Empresa_Tecnologia_ representa a associação entre empresas e tecnologias, onde muitas empresas podem utilizar várias tecnologias e várias tecnologia podem ser utilizadas por várias empresas(relação N,N).  

A tabela _Colaborador_ possui uma relação onde indica que muitos colaboradores podem fazer parte de uma Empresa(relação N,1).  

E uma tecnologia pode ser usada por muitas empresas(relação 1,N).  


---
### Simulando os registros:

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
Nome: Josean Borges  
Cargo: Analista de Dados  
ID_Empresa: 2  



Sistema RESILIADATA

