---
title: 'user: delta'
description: Obter usuários recém-criados, atualizados ou excluídos sem ter que realizar uma leitura completa de toda a coleção de usuários. Consulte controlar alterações para obter detalhes.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536998"
---
# <a name="user-delta"></a>user: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter usuários recém-criados, atualizados ou excluídos sem ter que realizar uma leitura completa de toda a coleção de usuários. Consulte [controlar alterações](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | User.Read, User.ReadWrite    |
|Aplicativo | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações nos usuários provoca uma rodada de uma ou mais chamadas de função **Delta** . Se você usar qualquer parâmetro de consulta (diferente `$deltatoken` de `$skiptoken`e), você deve especificá-lo na solicitação de **Delta** inicial. O Microsoft Graph codifica automaticamente qualquer parâmetro especificado na parte do token do URL `nextLink` ou `deltaLink` na resposta fornecida.

Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.

Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Este método oferece suporte a parâmetros de consulta OData opcionais para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.
- Há suporte limitado para `$filter`:
  - A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`. É possível filtrar vários objetos. Por exemplo, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Há um limite de 50 objetos filtrados.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |
| Preferir | retorno = mínimo <br><br>A especificação desse cabeçalho com uma solicitação que usa `deltaLink` um retornava apenas as propriedades do objeto que foram alteradas desde a última rodada. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](../resources/user.md) no corpo da resposta. A resposta também inclui uma `nextLink` URL ou uma `deltaLink` URL.

- Se uma `nextLink` URL for retornada:
  - Isso indica que há outras páginas de dados a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.
  - A resposta inclui o mesmo conjunto de propriedades que na solicitação de consulta Delta inicial. Isso permite que você capture o estado atual completo dos objetos ao iniciar o ciclo Delta.

- Se uma `deltaLink` URL for retornada:
  - Isso indica que não há mais dados sobre o estado existente do recurso a ser retornado. Salve e use a `deltaLink` URL para saber mais sobre as alterações no recurso na próxima rodada.
  - Você tem a opção de especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta somente para as propriedades que foram alteradas desde o momento `deltaLink` em que foi emitido.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Padrão: retornar as mesmas propriedades que a solicitação Delta inicial

Por padrão, as solicitações usando `deltaLink` uma `nextLink` ou retornam as mesmas propriedades selecionadas na consulta Delta inicial das seguintes maneiras:

- Se a propriedade tiver sido alterada, o novo valor será incluído na resposta. Isso inclui propriedades que estão sendo definidas como valor nulo.
- Se a propriedade não tiver sido alterada, o valor antigo será incluído na resposta.
- Se a propriedade nunca tiver sido definida antes de não ser incluída na resposta.


> **Observação:** Com esse comportamento, observando a resposta, não é possível dizer se uma propriedade está sendo alterada ou não. Além disso, as respostas Delta tendem a ser grandes porque elas contêm todos os valores de propriedade, conforme mostrado no [segundo exemplo](#request-2) abaixo.

#### <a name="alternative-return-only-the-changed-properties"></a>Alternativa: retornar somente as propriedades alteradas

Adicionar um cabeçalho de solicitação opcional `prefer:return=minimal` --resulta no seguinte comportamento:

- Se a propriedade tiver sido alterada, o novo valor será incluído na resposta. Isso inclui propriedades que estão sendo definidas como valor nulo.
- Se a propriedade não tiver sido alterada, a propriedade não será incluída na resposta. (Diferente do comportamento padrão.)

> **Observação:** O cabeçalho pode ser adicionado a uma `deltaLink` solicitação em um determinado momento no ciclo Delta. O cabeçalho afeta apenas o conjunto de propriedades incluído na resposta e não afeta como a consulta Delta é executada. ConFira o [terceiro exemplo](#request-3) abaixo.

### <a name="example"></a>Exemplo

#### <a name="request-1"></a>Solicitação 1

Este é um exemplo de solicitação. Não há nenhum `$select` parâmetro, portanto, um conjunto padrão de propriedades é rastreado e retornado.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a>Resposta 1

Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

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

#### <a name="request-2"></a>Solicitação 2

O exemplo a seguir mostra a solicitação inicial selecionando 3 Propriedades para o controle de alterações, com comportamento de resposta padrão:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a>Resposta 2

Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta. Observe que todas as 3 propriedades estão incluídas na resposta e não são conhecidas quais foram alteradas desde que `deltaLink` foram obtidas.

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
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a>Solicitação 3

O exemplo a seguir mostra a solicitação inicial selecionando 3 Propriedades para controle de alterações, com comportamento de resposta mínimo alternativo:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a>Resposta 3

Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta. Observe que a `mobilePhone` propriedade não é incluída, o que significa que ela não foi alterada desde a última consulta Delta; `displayName` e `jobTitle` são incluídos, o que significa que seus valores foram alterados.

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
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- [Usar a consulta Delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).
- [Obter alterações incrementais para usuários](/graph/delta-query-users).

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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
