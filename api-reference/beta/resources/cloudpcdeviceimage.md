---
title: Tipo de recurso cloudPcDeviceImage
description: Representa o recurso de imagem no Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 83dfce84c3a1c911d51ca7cf66d864945f3391f9
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533917"
---
# <a name="cloudpcdeviceimage-resource-type"></a>Tipo de recurso cloudPcDeviceImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso de imagem em um computador cloud.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceImages](../api/virtualendpoint-list-deviceimages.md)|[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Listar as propriedades e as relações dos [objetos cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Obter cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Leia as propriedades e as relações de um [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Criar cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Excluir cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|Nenhum|[Exclua um objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[Coleção cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)|Obter [objetos cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)|
|[Reupload cloudPcDeviceImage](../api/cloudpcdeviceimage-reupload.md)|Nenhum|Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do recurso de imagem no Cloud PC. Somente leitura.|
|sourceImageResourceId|Cadeia de Caracteres|A ID do recurso de imagem de origem no Azure. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|displayName|String|O nome de exibição da imagem.|
|versão|String|A versão da imagem. Por exemplo: 0.0.1, 1.5.13.|
|osBuildNumber|Cadeia de Caracteres|A versão de com build do sistema operacional da imagem. Por exemplo: 1909.|
|operatingSystem|String|O sistema operacional da imagem. Por exemplo: Windows 10 Enterprise.|
|lastModifiedDateTime|DateTimeOffset|Os dados e a hora em que a imagem foi modificada pela última vez. O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'.|
|status|cloudPcDeviceImageStatus|O status da imagem no Cloud PC. Os valores possíveis são: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Os detalhes do status da imagem, que indica por que o carregamento falhou, se aplicável. Os valores possíveis são: `internalServerError`, `sourceImageNotFound`, `osVersionNotSupported`, e `sourceImageInvalid`.|

### <a name="cloudpcdeviceimagestatus-values"></a>valores cloudPcDeviceImageStatus

|Member|Descrição|
|:---|:---|
|pendente|O carregamento da imagem está em andamento.|
|ready|A imagem está pronta para uso em PCs de nuvem.|
|failed|A imagem não pôde ser carregada. |

### <a name="cloudpcdeviceimagestatusdetails-values"></a>valores cloudPcDeviceImageStatusDetails

|Member|Descrição|
|:---|:---|
|internalServerError|Houve um erro de servidor interno durante o processamento da imagem.|
|sourceImageNotFound|A imagem de origem está inacessível ou não encontrada.|
|osVersionNotSupported| A versão do sistema operacional não é suportada.|
|sourceImageInvalid|A imagem de origem não é válida para provisionar uma Windows VM com ela.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
