---
title: Listar domainNameReferences
description: Recupere uma lista de directoryObject com uma referência ao domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 87a244e1a89c3f23c184796777e027fd314dcfe992447c06618bfeef90e03132
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272036"
---
# <a name="list-domainnamereferences"></a>Listar domainNameReferences

Namespace: microsoft.graph

Recupere uma lista [de directoryObject](../resources/directoryobject.md) com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Domain.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{domain-id}/domainNameReferences
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com/domainNameReferences
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domainnamereferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f/Microsoft.DirectoryServices.User",
      "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "accountEnabled": true,
      "city": "Nairobi",
      "createdDateTime": "2021-04-14T05:26:16Z",
      "country": "Kenya",
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "mail": "AdeleV@Contoso.com",
      "mailNickname": "AdeleV"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/eac82bd3-931c-4d47-9e68-735595a8eb8a/Microsoft.DirectoryServices.Group",
      "id": "eac82bd3-931c-4d47-9e68-735595a8eb8a",
      "createdDateTime": "2021-04-14T06:59:47Z",
      "createdByAppId": "00000005-0000-0ff1-ce00-000000000000",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "description": "Contribute your ideas and ask your questions to our leadership team. And tune in for regular Employee Q & A live events. You can learn more about what",
      "displayName": "CEO Connection",
      "expirationDateTime": "2021-10-11T06:59:47Z",
      "groupTypes": [
        "Unified"
      ],
      "mail": "ceoconnection@Contoso.com",
      "mailEnabled": true,
      "mailNickname": "ceoconnection",
      "resourceBehaviorOptions": [
        "CalendarMemberReadOnly"
      ],
      "visibility": "Public",
      "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
