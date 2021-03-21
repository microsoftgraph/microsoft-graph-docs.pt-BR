---
title: Tipo de recurso cloudPcDeviceImage
description: Representa o recurso de imagem no computador de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d4a88bb4d826ead30d1d739e696dec76df5cbb2f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957062"
---
# <a name="cloudpcdeviceimage-resource-type"></a>Tipo de recurso cloudPcDeviceImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso de imagem no computador de nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceImages](../api/virtualendpoint-list-deviceimages.md)|[Coleção cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Listar as propriedades e as relações dos [objetos cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Obter cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Leia as propriedades e as relações de um [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Criar cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Crie um novo [objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Excluir cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|Nenhum|[Exclua um objeto cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[Coleção cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)|Obter [objetos cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do recurso de imagem no computador de nuvem. Somente leitura.|
|sourceImageResourceId|Cadeia de caracteres|A ID do recurso de imagem de origem no Azure. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|displayName|Cadeia de caracteres|O nome de exibição da imagem.|
|versão|String|A versão da imagem. Por exemplo: 0.0.1, 1.5.13.|
|osBuildNumber|Cadeia de caracteres|A versão de com build do sistema operacional da imagem. Por exemplo: 1909.|
|operatingSystem|String|O sistema operacional da imagem. Por exemplo: Windows 10 Enterprise.|
|lastModifiedDateTime|DateTimeOffset|Os dados e a hora em que a imagem foi modificada pela última vez. O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'.|
|status|cloudPcDeviceImageStatus|O status da imagem no computador de nuvem. Os valores possíveis são: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Os detalhes do status da imagem, que indica por que o carregamento falhou, se aplicável. Os valores possíveis são: `internalServerError` e `sourceImageNotFound`.|

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
|sourceImageInvalid|A imagem de origem não é válida para provisionar uma VM do Windows com ela.|

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
