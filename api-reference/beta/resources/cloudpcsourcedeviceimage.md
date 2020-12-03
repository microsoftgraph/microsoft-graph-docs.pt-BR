---
title: tipo de recurso cloudPcSourceDeviceImage
description: 'A imagem de origem associada à sua assinatura do Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c944ab1a634d10e978c6ce1620ebe1accc5e4359
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563741"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>tipo de recurso cloudPcSourceDeviceImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A imagem de origem associada à sua assinatura do Azure.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da imagem de origem.|
|displayName|String|O nome de exibição da imagem de origem.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage",
  "baseType": "microsoft.graph.entity"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
