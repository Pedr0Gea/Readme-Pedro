# Projeto da oficina mecânica do Pedrão

## Aplicação
Vamos criar uma aplicação para gerenciar uma oficina mecãica.

## Tecnologias utilizadas
Para a construção da aplicação usaremos as linguagens , HTML, CSS, PHP, MYQSL e JavaScript.

### Banco de dados  do projeto

```sql
create database oficina_mecanica
```
---

### Criação da tabela peças

```sql
CREATE TABLE `oficina_mecanica`.`tb_pecas` (
    `codigo` INT NOT NULL AUTO_INCREMENT , 
    `descricao` VARCHAR(40) NOT NULL , 
    `unidade` VARCHAR(10) NOT NULL , 
    `preco` DECIMAL(10,2) NOT NULL , 
    PRIMARY KEY (`codigo`));
```

#### Organização dos arquivos
O cadastro de peças deve possuir os seguintes arquivos
| Arquivo  | Descrição |
| ------------- | ------------- |
| form_peca.php  | Formulário para cadastro de peça  |
| inclui_peca.php  | Arquivo que insere os dados da peça na tabela  |
| lista_peca.php  | Arquivo que exibe o cadastro de peça  |
| edita_peca.php  | Formulário para alteração do cadastro de peça  |
| salva_peca.php  | Arquivo que atualiza os dados da peça na tabela  |
--- 

### Criação da tabela de clientes

```sql
CREATE TABLE `oficina_mecanica`.`tb_clientes` (
    `codigo` INT NOT NULL AUTO_INCREMENT , 
    `nome` VARCHAR(50) NOT NULL , 
    `cpf` VARCHAR(20) NOT NULL ,
    `endereco` VARCHAR(60) NOT NULL ,
    `telefone` VARCHAR(15) NOT NULL , 
    `email` VARCHAR(40) NOT NULL ,
    `sexo` VARCHAR(40) NOT NULL ,
    `datanasc` VARCHAR(40) NOT NULL ,
    PRIMARY KEY (`codigo`));
```

#### Organização dos arquivos
O cadastro de clientes deve possuir os seguintes arquivos
| Arquivo  | Descrição |
| ------------- | ------------- |
| form_cliente.php  | Formulário para cadastro de cliente  |
| inclui_cliente.php  | Arquivo que insere os dados do cliente na tabela  |
| lista_clientes.php  | Arquivo que exibe o cadastro de cliente  |
| editacliente.php  | Formulário para alteração do cadastro de cliente  |
| salva_clientes.php  | Arquivo que atualiza os dados do cliente na tabela  |

---

### Criação da tabela de marcas

```sql
CREATE TABLE `oficina_mecanica`.`tb_marcas` (
    `codigo` INT NOT NULL AUTO_INCREMENT , 
    `descricao` VARCHAR(40) NOT NULL , 
    PRIMARY KEY (`codigo`));
```

#### Organização dos arquivos
O cadastro de marcas deve possuir os seguintes arquivos
| Arquivo  | Descrição |
| ------------- | ------------- |
| form_marca.php  | Formulário para cadastro de marca  |
| inclui_marca.php  | Arquivo que insere os dados da marca na tabela  |
| lista_marcas.php  | Arquivo que exibe o cadastro de marcas  |
| editamarca.php  | Formulário para alteração do cadastro de marca  |
| salva_marcas.php  | Arquivo que atualiza os dados da marca na tabela  |
---

