# Bruno API Scenarios

Collection do Bruno gerada a partir dos cenarios descritos em:

- `stk_cep_v2.md`
- `stk_clima.txt`
- `stk_feriados.md`
- `stk_isbn.md`

## Como usar

1. Abra a pasta `bruno-api-tests` no Bruno.
2. Selecione o ambiente `dev`.
3. Ajuste `baseUrl` se necessario.
4. Ajuste `validCityCode` se quiser validar os cenarios de clima com uma cidade conhecida na base CPTEC.
5. Execute os requests individualmente ou por pasta.

## Observacoes

- Os cenarios de sucesso usam exemplos consistentes com os markdowns.
- Em alguns cenarios validos de ISBN, o markdown admite `Sucesso/404`; nesses casos os testes aceitam ambas as respostas.
- Os cenarios de valor vazio ou nulo em parametros de path foram representados como chamada para o recurso sem o valor final no path.
- Os cenarios de clima usam `validCityCode` e `invalidCityCode` no ambiente para facilitar ajuste sem editar os requests.
