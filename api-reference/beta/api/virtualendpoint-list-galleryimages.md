---
title: List galleryImages
description: Listar as propriedades e relações das imagens da galeria da organização.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: df5b120c919017d0f87b855ec193f5bb5237dd36
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890455"
---
# <a name="list-galleryimages"></a>List galleryImages

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar as propriedades e as relações dos objetos [cloudPcGalleryImage.](../resources/cloudpcgalleryimage.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/galleryImages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece `$select` suporte e `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcgalleryimage"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/galleryImages
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcgalleryimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcgalleryimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcgalleryimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcgalleryimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcGalleryImage",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cloudPcGalleryImage",
    "value": [
        {
            "id":"MicrosoftWindowsDesktop_windows-ent-cpc_19h2-ent-cpc-os",
            "displayName":"Windows 10 Enterprise + OS Optimizations 1909",
            "offerDisplayName":"Windows 10 Enterprise + OS Optimizations",
            "skuDisplayName":"1909",
            "publisher":"MicrosoftWindowsDesktop",
            "offer":"windows-ent-cpc",
            "sku":"19h2-ent-cpc-os",
            "recommendedSku":"light",
            "status":"supported",
            "sizeInGB":64,
            "startDate":"2019-11-12",
            "endDate":"2022-05-10",
            "expiredDate":"2022-11-10"
        },
        {
            "id":"MicrosoftWindowsDesktop_windows-ent-cpc_20h1-ent-cpc-os",
            "displayName":"Windows 10 Enterprise + OS Optimizations 2004",
            "offerDisplayName":"Windows 10 Enterprise + OS Optimizations",
            "skuDisplayName":"2004",
            "publisher":"MicrosoftWindowsDesktop",
            "offer":"windows-ent-cpc",
            "sku":"20h1-ent-cpc-os",
            "recommendedSku":"light",
            "status":"supported",
            "sizeInGB":64,
            "startDate":"2020-05-27",
            "endDate":"2021-12-14",
            "expiredDate":"2022-06-14"
        }
   ]
}
```
