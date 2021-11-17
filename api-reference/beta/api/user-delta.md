---
title: 'user: delta'
description: Veja os usuários recentemente criados, atualizados ou excluídos sem ter que executar uma leitura completa da coleção de usuários inteira.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 3d540ebe848aa4af16cda1df90863aeb60b97c5f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009895"
---
# <a name="user-delta"></a>user: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Veja os usuários recentemente criados, atualizados ou excluídos sem ter que executar uma leitura completa da coleção de usuários inteira. Confira [controle de alterações](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.  |
|Aplicativo | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações em usuários corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.

Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.

Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Este método fornece suporte opcional a Parâmetros de Consulta OData para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.
- Há suporte limitado para `$filter`:
  - A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`. É possível filtrar vários objetos. Por exemplo, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Há um limite de 50 objetos filtrados.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |
| Preferir | return=minimal <br><br>Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/user.md) no corpo da resposta. A resposta também inclui uma URL `nextLink` ou `deltaLink`.

- Se uma URL `nextLink` for retornada:
  - Existem páginas de dados adicionais a recuperar na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.
  - A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial. Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.

- Se uma URL `deltaLink` for retornada:
  - Isso indica que não há mais nenhum dado a retornar sobre o estado do recurso. Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.
  - Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.

### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Padrão: retornar as mesmas propriedades de uma solicitação delta inicial

Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:

- Se a propriedade foi alterada, o novo valor será incluído na resposta. Isso inclui propriedades definidas com valor nulo.
- Se a propriedade não foi alterada, o valor antigo será incluído na resposta.
- Se a propriedade nunca foi definida anteriormente, de nenhuma forma será incluída na resposta.


> **Observação:** com esse comportamento, ao verificar a resposta, não será possível dizer se uma propriedade foi alterada ou não. Além disso, as respostas delta tendem a ser grandes porque contêm todos os valores de propriedades, como mostrado no [Exemplo 2](#example-2-selecting-three-properties).

### <a name="alternative-return-only-the-changed-properties"></a>Alternativa: retornar somente as propriedades alteradas

Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:

- Se a propriedade foi alterada, o novo valor será incluído na resposta. Isso inclui propriedades definidas com valor nulo.
- Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma. (Diferente do comportamento padrão.)

> **Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta. O cabeçalho afeta apenas o conjunto de propriedades incluídas na resposta e ele não afeta como a consulta delta é executada. Veja o [Exemplo 3](#example-3-alternative-minimal-response-behavior).

## <a name="examples"></a>Exemplos

### <a name="example-1-default-properties"></a>Exemplo 1: Propriedades padrão

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Não há nenhum parâmetro `$select`, assim um conjunto padrão de propriedades será controlado e retornado.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "+1 425 555 0109"
      ],
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "jobTitle": "Retail Manager",
      "mail": "AdeleV@contoso.onmicrosoft.com",
      "mobilePhone": "+1 425 555 0109",
      "officeLocation": "18/2111",
      "preferredLanguage": "en-US",
      "surname": "Vance",
      "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
      "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
    }
  ]
}
```

### <a name="example-2-selecting-three-properties"></a>Exemplo 2: Escolher três propriedades

#### <a name="request"></a>Solicitação

O próximo exemplo mostra uma solicitação inicial selecionando três propriedades para controle de alterações com comportamento de resposta padrão.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-delta-select-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta. Observe que todas as três propriedades foram incluídas na resposta e não se sabe quais foram alteradas desde que o `deltaLink` foi obtido.

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Adele Vance",
      "jobTitle": "Retail Manager",
      "mobilePhone": "+1 425 555 0109"
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a>Exemplo 3: Comportamento de resposta mínimo alternativo

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação inicial selecionando três propriedades para controle de alterações com o comportamento de resposta mínima alternativa.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-delta-minimal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta. Observe que a propriedade `mobilePhone` não foi incluída, ou seja, não foi alterada desde a última consulta delta; `displayName` e `jobTitle` foram incluídas, o que significa que os valores foram alterados.

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Vance Adele",
      "jobTitle": "Product Marketing Manager"
    }
  ]
}
```
## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).
- [Obter as alterações incrementais para usuários](/graph/delta-query-users).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


