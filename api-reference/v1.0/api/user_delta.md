# <a name="user-delta"></a>user: delta

A [consulta delta](../../../concepts/delta_query_overview.md) permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Para descobrir as alterações nos usuários, realize uma solicitação usando a função *delta*. Confira [Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes.

## <a name="prerequisites"></a>Pré-requisitos

Um dos seguintes **escopos** é obrigatório para executar esta API: *User.Read; User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*

## <a name="http-request"></a>Solicitação HTTP

Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários. 

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

### <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações em usuários corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.|
| $skiptoken | string | Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 
- Suporte à consulta delta `$select`, `$top` e `$expand` para mensagens. 
- Há suporte limitado para `$orderby`: A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida. 
- Não há suporte DAV para `$search`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção [user](../resources/user.md) no corpo da resposta. A resposta também inclui uma URL nextLink ou uma URL deltaLink. 

- Se uma URL nextLink é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL nextLink até uma URL deltaLink ser incluída na resposta.

- Se uma URL deltaLink for retornada, não haverá mais dados sobre o estado existente do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso.

Confira:</br>
- [Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes</br>
- [Obter as alterações incrementais para usuários](../../../concepts/delta_query_users.md) para solicitações de um exemplo.</br>

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/delta
```

##### <a name="response"></a>Resposta
Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->