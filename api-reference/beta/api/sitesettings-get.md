---
title: Obter siteSettings
description: Obtenha as configurações de um site.
author: k-tsoi
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: fe05b525d506fb3192244b40a784dc7971843bea
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211176"
---
# <a name="get-sitesettings"></a>Obter siteSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as configurações de um [site].

>**Nota:** Atualmente, essa API só está disponível em SharePoint e OneDrive for Business.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:--------------------------------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Sites.Read.All, Sites.ReadWrite.All         |
|Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
|Aplicativo                            | Sites.Read.All, Sites.ReadWrite.All         |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/settings
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto siteSettings](../resources/sitesettings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sitesettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/03164a2b-a288-486a-993e-c41454113e2a/settings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sitesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sitesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sitesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sitesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
  "languageTag": "String",
  "timeZone": "String"
  }
}
```

[site]: ../resources/site.md
