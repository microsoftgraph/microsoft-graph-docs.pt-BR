---
title: Tipo de recurso cloudPcDeviceImage
description: Representa o recurso de imagem no Cloud PC.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: eb46059f675fc392fe0ec3c83d7c3cb6ba60e869
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567395"
---
# <a name="cloudpcdeviceimage-resource-type"></a>Tipo de recurso cloudPcDeviceImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso de imagem em um computador cloud.

## <a name="methods"></a>Methods

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
|displayName|Cadeia de caracteres|O nome de exibição da imagem.|
|expirationDate|Data|A data em que a imagem ficou indisponível.|
|id|Cadeia de caracteres|Identificador exclusivo do recurso de imagem no Cloud PC. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Os dados e a hora em que a imagem foi modificada pela última vez. O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como '2014-01-01T00:00:00Z'.|
|operatingSystem|String|O sistema operacional da imagem. Por exemplo: Windows 10 Enterprise.|
|osBuildNumber|Cadeia de caracteres|A versão de com build do sistema operacional da imagem. Por exemplo: 1909.|
|osStatus|[cloudPcDeviceImageOsStatus](#cloudpcdeviceimageosstatus-values)|O status do sistema operacional dessa imagem. Os valores possíveis são: `supported`, `supportedWithWarning`, `unknownFutureValue`.|
|sourceImageResourceId|Cadeia de caracteres|A ID do recurso de imagem de origem no Azure. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|status|[cloudPcDeviceImageStatus](#cloudpcdeviceimagestatus-values)|O status da imagem no Cloud PC. Os valores possíveis são: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Os detalhes do status da imagem, que indica por que o carregamento falhou, se aplicável. Os valores possíveis são: `internalServerError` , , , e `sourceImageNotFound` `osVersionNotSupported` `sourceImageInvalid` `sourceImageNotGeneralized` .|
|versão|String|A versão da imagem. Por exemplo, 0.0.1, 1.5.13.|

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
|sourceImageNotGeneralized|A imagem carregada não foi generalizada. Reupload the image after running the sysprep/generalize command. Para saber mais, confira Remover informações específicas do computador [generalizando uma VM antes de criar uma imagem](/azure/virtual-machines/generalize).|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="cloudpcdeviceimageosstatus-values"></a>valores cloudPcDeviceImageOsStatus

|Member|Descrição|
|:---|:---|
|com suporte|A imagem do dispositivo está ativa e pronta para ser usada para provisionamento.|
|supportedWithWarning|A imagem do dispositivo expirou, mas o Cloud PC continuará a dar suporte. Se os usuários continuarem a usar, talvez não sejam capazes de obter atualizações de segurança.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

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
  "sourceImageResourceId": "String",
  "expirationDate":"String (timestamp)",
  "osStatus":"String"
}
```
