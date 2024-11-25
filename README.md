ANIMAIS ENCONTRADOS 

CREATE DATABASE father_pets;

USE father_pets;

CREATE TABLE animais_encontrados (
    id INT AUTO_INCREMENT PRIMARY KEY,           
    nome VARCHAR(100) NOT NULL,                
    email_encontrou VARCHAR(150) NOT NULL,      
    telefone_encontrou VARCHAR(15) NOT NULL,    
    tipo ENUM('Cachorro', 'Gato', 'Outro') NOT NULL, 
    sexo ENUM('Macho', 'Fêmea') NOT NULL,     
    local_cidade VARCHAR(100) NOT NULL,        
    local_estado VARCHAR(100) NOT NULL,
    referencia_local TEXT,                      
    descricao_pet TEXT NOT NULL,                
    foto_pet TEXT,                               
    data_registro TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);



ANIMAIS 

CREATE DATABASE father_pets;

USE father_pets;

CREATE TABLE animais (
    id INT AUTO_INCREMENT PRIMARY KEY,       
    nome VARCHAR(100) NOT NULL,              
    tipo ENUM('Cachorro', 'Gato', 'Outro') NOT NULL,
    sexo ENUM('Macho', 'Fêmea') NOT NULL,    
    porte ENUM('Pequeno', 'Médio', 'Grande') NOT NULL, 
    cidade VARCHAR(100) NOT NULL,            
    estado VARCHAR(100) NOT NULL,             
    foto TEXT,                              
    nome_usuario VARCHAR(100) NOT NULL,      
    email_usuario VARCHAR(150) NOT NULL,     
    telefone_usuario VARCHAR(15) NOT NULL,   
    data_registro TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
  
usuário

CREATE DATABASE father_pets;

USE father_pets;

CREATE TABLE usuarios (
    id INT AUTO_INCREMENT PRIMARY KEY,               
    primeiro_nome VARCHAR(50) NOT NULL,              
    sobrenome VARCHAR(255),                         
    email VARCHAR(100) NOT NULL,                    
    senha VARCHAR(255) NOT NULL,                   
    genero ENUM('Feminino', 'Masculino', 'Outros', 'Prefiro não dizer'), 
    criado_em TIMESTAMP DEFAULT CURRENT_TIMESTAMP, 
    token_recuperacao VARCHAR(255),                 
    token_expiracao DATETIME,                       
    celular VARCHAR(20)                          
);

