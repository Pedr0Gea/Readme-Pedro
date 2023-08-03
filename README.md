# Projeto da oficina mecânica do Pedrão

## Aplicação
Vamos criar uma aplicação para gerenciar uma oficina mecânica.

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
| editapeca.php  | Formulário para alteração do cadastro de peça  |
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

### Criação da tabela modelos

```sql
CREATE TABLE `oficina_mecanica`.`tb_modelos` (
    `codigo` INT NOT NULL AUTO_INCREMENT , 
    `descricao` VARCHAR(40) NOT NULL , 
    `cod_marca` INT NOT NULL ,
    PRIMARY KEY (`codigo`));
```

### Organização dos arquivos
O cadastro de marcas deve possuir os seguintes arquivos
| Arquivo  | Descrição |
| ------------- | ------------- |
| form_modelo.php  | Formulário para cadastro de marca  |
| inclui_modelo.php  | Arquivo que insere os dados da marca na tabela  |
| lista_modelos.php  | Arquivo que exibe o cadastro de marcas  |
| editamodelo.php  | Formulário para alteração do cadastro de marca  |
| salva_modelos.php  | Arquivo que atualiza os dados da marca na tabela  |
---

### Criação da tabela veículos

```sql
CREATE TABLE `oficina_mecanica`.`tb_veiculos` (
    `codigo` INT NOT NULL AUTO_INCREMENT , 
    `placa` VARCHAR(10) NOT NULL , 
    `cod_modelo` INT NOT NULL ,
    `cor` VARCHAR(20) , 
     PRIMARY KEY (`codigo`));
```

#### Organização dos arquivos (veículos)
O cadastro de veículos deve possuir os seguintes arquivos
| Arquivo  | Descrição |
| ------------- | ------------- |
| form_veiculo.php  | Formulário para cadastro de veículo  |
| inclui_veiculo.php  | Arquivo que insere os dados do veículo na tabela  |
| lista_veiculos.php  | Arquivo que exibe o cadastro de veículos  |
| editaveiculo.php  | Formulário para alteração do cadastro de veículo  |
| salva_veiculos.php  | Arquivo que atualiza os dados do veículo na tabela  |
---

