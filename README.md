sql запросы 
USE [dminin]
GO

INSERT INTO [dbo].[ProductType]
           ([Title]
           ,[DefectedPercent])
  SELECT 
     distinct [Тип продукции],0
     
  FROM [dbo].[products_k_import$]
