# Criação de um Star Schema utilizando DAX
Criação de um esquema dimensional – star schema – utilizando DAX.

## Visualização: 

Implementação gráfica do star schema com DAX.  
![star_schema_dax](https://github.com/user-attachments/assets/529ab550-79be-4c16-bc5b-7a770794f32a)

## Construção do diagrama:
Foram criadas as tabelas a partir do modelo Financials do Power BI:  
- D_Produtos (ID_produto, Produto, Média de Unidades Vendidas, Médias do valor de vendas, Mediana do valor de vendas, Valor máximo de Venda, Valor mínimo de Venda)  
- D_Produtos_Detalhes(ID_produtos, Discount Band, Sale Price, Units Sold, Manufactoring Price)  
- D_Descontos (ID_produto, Discount, Discount Band)
- D_Calendário – Criada por DAX com calendar()  
- F_Vendas (SK_ID , ID_Produto, Produto, Units Sold, Sales Price, Discount Band, Segment, Country, Salers, Profit, Date (campos))  
- D_Detalhes (*)  
- D_Categoria (*) 
  
Referência: [DIO: Power BI Analyst](https://github.com/julianazanelatto/power_bi_analyst/tree/main/M%C3%B3dulo%204)
