# Bigrama Matcher

O Bigrama Matcher é uma ferramenta Python para localização e correspondência de bigramas entre dois conjuntos de dados, permitindo encontrar bigramas semelhantes e analisar sua presença em diferentes conjuntos.

## Descrição

A biblioteca utiliza a biblioteca FuzzyWuzzy para cálculos de similaridade e oferece opções para correspondência exata, correspondência de n-gramas e ajuste fino de parâmetros de similaridade.

## Funcionalidades

- Correspondência de bigramas entre dois conjuntos de dados.
- Suporte para correspondência exata ou fuzzy.
- Opção para correspondência de n-gramas.
- Ajuste do limiar de similaridade para personalização da correspondência.
- Análise de presença e localização de bigramas semelhantes.

## Como Usar

```python
# Exemplo de uso:
from bigrama_matcher import BigramaMatcher

# Carregar seus conjuntos de dados (df1 e df2)
bigrama_matcher = BigramaMatcher(df1, df2, column_name_df1='Bigramas Preprocessados', column_name_df2='Bigramas Preprocessados', fuzz_threshold=80)
result_df = bigrama_matcher.match_bigrams()

# Exibir o resultado
print(result_df)
```

## Parâmetros

- `df1`: DataFrame do primeiro conjunto de dados.
- `df2`: DataFrame do segundo conjunto de dados.
- `column_name_df1`: Nome da coluna contendo os bigramas no DataFrame 1.
- `column_name_df2`: Nome da coluna contendo os bigramas no DataFrame 2.
- `fuzz_threshold`: Limiar de similaridade para correspondência fuzzy (padrão: 70).

## Contribuição

Contribuições são bem-vindas! Por favor, abra uma issue ou envie um pull request para melhorias ou correções.

## Licença

Este projeto é licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para detalhes.


