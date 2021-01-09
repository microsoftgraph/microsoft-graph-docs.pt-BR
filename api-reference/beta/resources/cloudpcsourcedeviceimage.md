---
title: Tipo de recurso cloudPcSourceDeviceImage
description: 'A imagem de origem associada à sua assinatura do Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b0c656142ddad5af3d0af7778d0ae04f0c5d7b4
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790738"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>Tipo de recurso cloudPcSourceDeviceImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A imagem de origem associada à sua assinatura do Azure.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da imagem de origem.|
|displayName|Cadeia de caracteres|O nome de exibição da imagem de origem.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
