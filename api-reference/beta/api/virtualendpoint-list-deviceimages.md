---
title: Listar cloudPcDeviceImages
description: Listar as propriedades e as relações das imagens do sistema operacional carregadas no Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4d392331b2cb07446374275d0ffb8e606fe7d99d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378251"
---
# <a name="list-deviceimages"></a>Listar deviceImages

Namespace: microsoft.graph

Liste as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) (imagens de so) carregadas no Cloud PC.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC. ReadWrite. All, CloudPC. Read. All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte a `$select` `$filter` parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
      "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
      "displayName": "Display Name value",
      "osBuildNumber": "OS Build Number value",
      "operatingSystem": "Operating System value",
      "version": "Version value",
      "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "lastModifiedDateTime": "2020-11-03T07:03:44Z",
      "status": "pending",
      "statusDetails": null
    }
  ]
}
```
