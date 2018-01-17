# Entity Framework Core Trainning
Projeto de aprendizado e testes com Entity Framework Core que visa desenvolver uma arquitetura concisa e desacoplada de componentes de acesso a dados.

## Estrutura��o da solu��o
Projeto | Prop�sito
-- | --
```EFCoreTrainning.Domain```| Cont�m classes POCO do dom�nio do neg�cio.
```EFCoreTrainning.DataAccess```| Camada respons�vel pelas opera��es de CRUD no banco de dados.
```EFCoreTrainning.DataAccess.Tests```| Projeto de testes unit�rios do EFCoreTrainning.DataAccess.
```EFCoreTrainning.WebApi```| Aplica��o da camada de apresenta��o para expor as funcionalidades do sistema.

## Esquema de depend�ncias
Projeto | Depende de
-- | --
```EFCoreTrainning.Domain```| _nenhuma depend�ncia_
```EFCoreTrainning.DataAccess```| ```EFCoreTrainning.Domain```
```EFCoreTrainning.WebApi```| ```EFCoreTrainning.Domain``` e ```EFCoreTrainning.DataAccess```