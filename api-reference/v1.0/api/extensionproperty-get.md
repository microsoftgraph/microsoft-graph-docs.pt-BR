---
title: Obter extensionProperty
description: Ler um objeto extensionProperty.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7e3e0cc06496b3328ab79b1058bb15f747645238
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2022
ms.locfileid: "65016803"
---
# <a name="get-extensionproperty"></a>Obter extensionProperty
Namespace: microsoft.graph

Ler um [objeto extensionProperty](../resources/extensionproperty.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Application.Read.All, Application.ReadWrite.All    |
|Aplicativo | Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applications/{application ObjectId}/extensionProperties/{extensionPropertyId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [extensionProperty](../resources/extensionproperty.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperty"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties/1f0f15e3-925d-40f0-8fc8-9d3ad135bce0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-extensionproperty-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-extensionproperty-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications('fd918e4b-c821-4efb-b50a-5eddd23afc6f')/extensionProperties/$entity",
    "id": "1f0f15e3-925d-40f0-8fc8-9d3ad135bce0",
    "deletedDateTime": null,
    "appDisplayName": "b2c-extensions-app. Do not modify. Used by AADB2C for storing user data.",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "name": "extension_25883231668a43a780b25685c3f874bc_cpiminternal_useAccountEnabledForPhone",
    "targetObjects": [
        "User"
    ]
}
```

