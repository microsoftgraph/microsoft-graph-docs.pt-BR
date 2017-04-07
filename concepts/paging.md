
# <a name="paging-microsoft-graph-data-in-your-app"></a>Paginação de dados do Microsoft Graph em seu aplicativo 
 
Quando as solicitações do Microsoft Graph retornam muitas informações para mostrar em uma página, você pode usar paginação para dividir as informações em partes gerenciáveis. 

Você pode avançar e voltar as páginas em respostas do Microsoft Graph. Uma resposta que contém resultados paginados inclui um token skip (**odata.nextLink**) que permite que você obtenha a próxima página de resultados. Esse token skip pode ser combinado a um argumento de consulta **previous-page=true** para retroceder pelas páginas.

O exemplo de solicitação a seguir mostra como avançar nas páginas:

```
https://graph.microsoft.com/v1.0/users?$top=5$skiptoken=X'4453707402.....0000'
```
O parâmetro **$skiptoken** da resposta anterior é incluído e permite que você obtenha a próxima página de resultados.

O exemplo de solicitação a seguir mostra como retroceder nas páginas:

```
https://graph.microsoft.com/v1.0/users?$top=5$skiptoken=X'4453707.....00000'&previous-page=true
```
O parâmetro **$skiptoken** da resposta anterior está incluído. Quando isso for combinado ao parâmetro **&previous-page=true**, a página anterior de resultados será recuperada.

A seguir estão as etapas de solicitação/resposta para avançar e voltar as páginas:

1. Uma solicitação é feita para obter uma lista dos 10 primeiros usuários em 15. A resposta contém um token skip para indicar a página final do 10 usuários.
2. Para obter os cinco usuários finais, outra solicitação é feita contendo o token skip retornado da resposta anterior.
3. Para voltar a página, uma solicitação é feita usando o token skip retornado na etapa 1 e o parâmetro **&previous-page=true** é adicionado à solicitação.
4. A resposta contém a página anterior (primeira) de 10 usuários. Em outro cenário onde houvesse mais páginas, um novo token skip poderia ser retornado. Esse novo token skip pode ser adicionado à solicitação junto com **&previous-page=true** para voltar a página novamente.

As seguintes restrições se aplicam às solicitações paginadas:

- O tamanho de página padrão é 100. O tamanho máximo de página é 999.
- As consultas em funções não dão suporte à paginação. Isso inclui os objetos de função de leitura e os membros de função.
- A paginação não tem suporte nas pesquisas de link, como consultas de membros do grupo.
