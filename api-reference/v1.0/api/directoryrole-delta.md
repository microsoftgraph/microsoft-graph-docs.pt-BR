---
title: 'directoryRole: delta'
description: Obter funções de diretório recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Using Delta Query para obter detalhes.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: afe1ebb541d8d83d7abd8d857383152e2756179b
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63669981"
---
# <a name="directoryrole-delta"></a>directoryRole: delta

Namespace: microsoft.graph

Obter funções de diretório recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte [Using Delta Query](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para começar a controlar as alterações, você faz uma solicitação incluindo a **função delta** no [recurso directoryRole](../resources/directoryrole.md) .

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **delta** anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **delta** anterior, indicando que há outras alterações a serem controladas na mesma coleção de recursos. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.

- Há suporte limitado para `$filter`:

  - A única expressão com suporte `$filter` é para controlar alterações para recursos específicos, por sua id:  `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`. O número de ids que você pode especificar é limitado pelo tamanho máximo da URL.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto da coleção directoryRole](../resources/directoryrole.md) no corpo da resposta. A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.

- Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.

- Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Salve `deltaLink` a URL e aplique-a na próxima chamada **delta** para saber mais sobre as alterações no recurso no futuro.

### <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryrole-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryrole-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pkXMyA5aFCIMmH1Kk1XEAnf2X-fodqXKXF03gYPQknSHRxogVsxvSq_26nhos-O2-shortened",
  "value": [
    {
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8",
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "members@delta": [
        {
          "@odata.type": "#microsoft.graph.user",
          "id": "bb165b45-151c-4cf6-9911-cd7188912848",
          "@removed": {
            "reason": "deleted"
          }
        }
      ]
    }
  ]
}
```

### <a name="see-also"></a>Confira também

- [Use a consulta delta para rastrear alterações no Microsoft Graph dados](/graph/delta-query-overview) para obter mais detalhes
- [Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

