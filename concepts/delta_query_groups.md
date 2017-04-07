# <a name="get-incremental-changes-for-groups-preview"></a>Obter as alterações incrementais para grupos (visualização)

A [Consulta delta](./delta_query_overview.md) permite que você consulte adições, exclusões ou atualizações de grupos, por meio de uma série de chamadas de função [delta](../api-reference/beta/api/group_delta.md). A consulta Delta permite que você descubra alterações em grupos sem ter que buscar todo o conjunto de grupos do Microsoft Graph e comparar as alterações.

A consulta delta oferece suporte à sincronização completa, que recupera todos os grupos em um locatário, e à sincronização incremental, que recupera somente os grupos que foram alterados desde a última sincronização. Normalmente, você faria uma sincronização completa inicial de todos os grupos e, logo após, obteria alterações incrementais para esses grupos periodicamente. 

## <a name="tracking-group-changes"></a>Controle de alterações de grupo

O controle de alterações de grupo corresponde a uma série de uma ou mais solicitações GET com a função **delta**. Criar uma solicitação GET é muito parecido com a forma de [listar grupos](../api-reference/beta/api/group_list.md), exceto se você incluir o seguinte:

- A função **delta**.
- Um [token de estado](./delta_query_overview.md) (_deltaToken_ ou _skipToken_) da chamada de função GET **delta** anterior.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma série de solicitações para rastrear as alterações nos grupos:

1. [Solicitação inicial](#initial-request) e [resposta](#initial-response)
2. [solicitação nextLink](#nextlink-request) e [resposta](#nextlink-response)
3. [Solicitação final nextLink](#final-nextlink-request) e [resposta](#final-nextlink-response)
4. [Solicitação deltaLink](#deltalink-request) e [resposta deltaLink](#deltalink-response)

## <a name="initial-request"></a>Solicitação inicial

Para iniciar o rastreamento de alterações no recurso de grupo, faça uma solicitação incluindo a função delta no recurso de grupo. 

Observe o seguinte:

- O parâmetro de consulta $select opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.
- A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados nas solicitações subsequentes.

``` http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description
```

### <a name="initial-response"></a>Resposta inicial

Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção [group](../api-reference/beta/resources/group.md) no corpo da resposta. Pressupondo que todo o conjunto de grupos é muito grande, a resposta também incluirá um token de estado nextLink.

Neste exemplo, uma URL nextLink é retornada indicando que não há páginas adicionais de dados a serem recuperados na sessão. O parâmetro de consulta $select da solicitação inicial é codificado na URL nextLink.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff"
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

## <a name="nextlink-request"></a>solicitação nextLink

A segunda solicitação especifica o `skipToken` retornado da resposta anterior. Observe que o parâmetro `$select` não é obrigatório, pois o `skipToken` codifica e o inclui.

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>Resposta nextLink

A resposta contém um `nextLink` e outro `skipToken`, indicando que não há mais grupos disponíveis. Continue fazendo solicitações usando a URL nextLink até uma URL deltaLink ser retornada na resposta.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957"
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Solicitação nextLink final

A terceira solicitação continua a usar os últimos `skipToken` retornados da última solicitação de sincronização. 

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Resposta nextLink final

Quando a URL deltaLink é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso. Salve o `deltaToken` e use-o na solicitação da URL para descobrir as alterações feitas nos grupos. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a>Solicitação deltaLink

Usando o `deltaToken` da [última resposta](#final-nextlink-response), você poderá obter grupos alterados (ao ser adicionado, excluído ou atualizado) desde o último pedido.

``` http
GET https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>Resposta deltaLink

Se não houve alterações, o mesmo `deltatoken` é retornado com nenhum resultado.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Se houve, o mesmo `deltatoken` é retornado incluindo um conjunto de grupos alterados.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup7",
      "description":"Employees in test group 7",
      "id":"f764235c-ffff-4843-a14a-1d8826967260"
    }
  ]
}
```

## <a name="see-also"></a>Veja também
Visão geral da [consulta delta do Microsoft Graph](../concepts/delta_query_overview.md).