# ModuloAPI

GRANT ALL PRIVILEGES ON *.* TO 'User'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;

show databases;

create
TABLE Produtos (
    id INT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    cor VARCHAR(10) NOT NULL,
    preco DECIMAL(10, 2) NOT NULL,
    quantidade INT NOT NULL,
    tamanho VARCHAR(5) NOT NULL,
    genero char(1) NOT NULL
);

INSERT INTO Produtos (id, nome, cor, preco, quantidade, tamanho, genero) VALUES
(1, 'Camiseta Básica', 'Branca', 29.90, 100, 'M', 'U'),
(2, 'Calça Jeans', 'Azul', 99.90, 50, 'L', 'M'),
(3, 'Vestido Floral', 'Vermelho', 79.90, 30, 'S', 'F'),
(4, 'Tênis Esportivo', 'Preto', 149.90, 75, '42', 'U'),
(5, 'Jaqueta de Couro', 'Marrom', 199.90, 20, 'XL', 'M');

SELECT * FROM Produtos;