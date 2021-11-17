---
title: Obter o status de um educationSynchronizationProfile
description: Obter o status de um perfil de sincronização de dados escolares específico no locatário. A resposta indicará o status da sincronização.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e16e62941b3aacdcf6954829ee4ca0fe5d5780a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986520"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a>Obter o status de um educationSynchronizationProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o status de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolares específico no locatário. A resposta indicará o status da sincronização.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                       | Permissões (da com menos para a com mais privilégios)                 |
| :------------------------------------ | :---------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)    | EduAdministration.Read, EduAdministration.ReadWrite         |
| Delegada (conta pessoal da Microsoft | Sem suporte.                                              |
| Aplicativo                           | EduAdministration.Read.All, EduAdministration.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Tipo   | Descrição               |
| :------------ | :----- | :------------------------ |
| Autorização | string | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-status-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationsynchronizationprofile-status-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2021-07-13T20:55:17.6475128Z",
    "lastActivityDateTime": "2021-07-13T20:55:17.6475128Z",
    "errorCount": 0,
    "statusMessage": "Processed 0 in the last hour.\r\nUpdated 0 in the last hour."
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


