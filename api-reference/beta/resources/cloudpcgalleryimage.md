---
title: Tipo de recurso cloudPcGalleryImage
description: Representa o recurso de imagem da galeria da organização atual.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7c539af9b8a31000af06cb88de594d80c4ea5eb5
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805532"
---
# <a name="cloudpcgalleryimage-resource-type"></a>Tipo de recurso cloudPcGalleryImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso de imagem da galeria da organização atual, que pode ser usado para provisionar um computador na nuvem.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List galleryImages](../api/virtualendpoint-list-deviceimages.md)|[Coleção cloudPcDeviceImage](../resources/cloudpcgalleryimage.md)|Listar as propriedades e as relações dos [objetos cloudPcDeviceImage.](../resources/cloudpcgalleryimage.md)|
|[Obter cloudPcGalleryImage](../api/cloudpcgalleryimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcgalleryimage.md)|Leia as propriedades e as relações de um [objeto cloudPcDeviceImage.](../resources/cloudpcgalleryimage.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição oficial da imagem da galeria. Somente leitura.|
|endDate|Data|A data em que essa imagem não está mais no suporte a longo prazo. O Cloud PC continuará fornecendo suporte a curto prazo. Somente leitura.|
|expirationDate|Data|A data em que a imagem não está mais disponível. Somente leitura.|
|id|Cadeia de caracteres|Identificador exclusivo do recurso de imagem da galeria no Cloud PC. Somente leitura.|
|offer|Cadeia de caracteres|O nome da oferta da imagem da galeria. Esse valor será passado para o Azure para obter o recurso de imagem. Somente leitura.|
|offerDisplayName|String|O nome da oferta de exibição oficial da imagem da galeria. Por exemplo, Windows 10 Enterprise + Otimizações do sistema operacional. Somente leitura.|
|publicador|String|O nome do editor da imagem da galeria. Esse valor será passado para o Azure para obter o recurso de imagem. Somente leitura.|
|recommendedSku|Cadeia de caracteres|SKU do Cloud PC recomendado para esta imagem de galeria. Somente leitura.|
|sizeInGB|Int32|O tamanho dessa imagem em gigabytes. Somente leitura.|
|sku|Cadeia de caracteres|O nome SKU da imagem da galeria. Esse valor será passado para o Azure para obter o recurso de imagem. Somente leitura.|
|skuDisplayName|Cadeia de caracteres|O nome da unidade de manutenção de ações de exibição oficial (SKU) desta imagem da galeria. Por exemplo, 2004. Somente leitura.|
|startDate|Data|A data em que a imagem fica disponível. Somente leitura.|
|status|cloudPcGalleryImageStatus|O status da imagem da galeria no Cloud PC. Os valores possíveis são: `supported`, `supportedWithWarning`, `notSupported`, `unknownFutureValue`. Somente leitura.|

### <a name="cloudpcgalleryimagestatus-values"></a>valores cloudPcGalleryImageStatus

|Member|Descrição|
|:---|:---|
|com suporte|A imagem da galeria está ativa e pronta para ser usada para provisionamento.|
|supportedWithWarning|A imagem da galeria expirou, mas o Cloud PC continuará com suporte por 6 meses, após o qual não terá suporte e não poderá ser usado.|
|notSupported|A imagem da galeria está sem suporte. |
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcGalleryImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName":"String",
  "offerDisplayName":"String",
  "skuDisplayName":"String",
  "publisher":"String",
  "offer":"String",
  "sku":"String",
  "recommendedSku":"String",
  "status":"String",
  "sizeInGB":"Int32",
  "startDate":"String (Date)",
  "endDate":"String (Date)",
  "expiredDate":"String (Date)"
}
```
