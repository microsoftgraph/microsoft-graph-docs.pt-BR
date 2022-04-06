---
title: Tipo de recurso cloudPcSourceDeviceImage
description: 'A imagem de origem associada à sua assinatura do Azure. '
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9bfdb8240d72a9b97f8b4dc89844734416576021
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723566"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>Tipo de recurso cloudPcSourceDeviceImage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A imagem de origem associada à sua assinatura do Azure.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da imagem de origem.|
|displayName|String|O nome de exibição da imagem de origem.|
|subscriptionId|String|A ID da assinatura que hospeda a imagem de origem.|
|subscriptionDisplayName|String|O nome de exibição da assinatura que hospeda a imagem de origem.|

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
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionDisplayName": "String"
}
```
