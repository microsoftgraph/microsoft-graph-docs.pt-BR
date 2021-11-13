---
title: Tipo de recurso qualityUpdateReference
description: Representa Windows 10 conteúdo de atualização de qualidade.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bae1315caf6efd2096f9039ca774db18f0b6b764
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890756"
---
# <a name="qualityupdatereference-resource-type"></a>Tipo de recurso qualityUpdateReference

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa Windows 10 conteúdo de atualização de qualidade.

Em uma implantação, a mesma referência de atualização de qualidade pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.

Herda de [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md). Tipo base [de expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classificação|microsoft.graph.windowsUpdates.qualityUpdateClassification|Especifica a classificação do conteúdo referenciado. Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**. Os valores possíveis são: `security` e `unknownFutureValue`.|
|releaseDateTime|DateTimeOffset|Especifica uma atualização de qualidade no determinado serviçoChannel com a classificação determinada por data (ou seja, a última atualização publicada na data especificada). O valor padrão é `security`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```

