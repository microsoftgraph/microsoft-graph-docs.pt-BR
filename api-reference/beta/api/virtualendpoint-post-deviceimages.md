---
title: Criar cloudPcDeviceImage
description: Carregue uma imagem de sistema operacional personalizada que possa ser provisionada posteriormente em PCs em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 7b2e60355bfe4db8eee014ac2290c83d146eea37
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378248"
---
# <a name="create-cloudpcdeviceimage"></a>Criar cloudPcDeviceImage

Namespace: microsoft.graph

Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) . Carregue uma imagem de sistema operacional personalizada que possa ser provisionada posteriormente em PCs em nuvem.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                |
| :------------ | :------------------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da imagem.|
|sourceImageResourceId|Cadeia de Caracteres|A ID do recurso de imagem de origem no Azure. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|operatingSystem|String|O sistema operacional da imagem. Por exemplo: Windows 10 Enterprise.|
|osBuildNumber|Cadeia de Caracteres|A versão de compilação do so da imagem. Por exemplo: 1909.|
|versão|String|A versão da imagem. Por exemplo: 0.0.1, 1.5.13.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_cloudpcdeviceimage_from_cloudpcdeviceimage"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 508

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
  "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
  "status": "pending",
  "statusDetails": null
}
```
