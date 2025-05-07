# Databricks-Dio

# Ler fonte de dados
diamonds_df = (spark.read
  .format("csv")
  .option("mode", "PERMISSIVE")
  .load("/databricks-datasets/Rdatasets/data-001/csv/ggplot2/diamonds.csv")
)

# Exibir Tabela
diamonds_df.show()
