---
title: Tipo de recurso expeditedQualityUpdateReference
description: Representa Windows 10 conteúdo de atualização de qualidade para acelerar.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: c3313483305613cf684b066f2ba9569676974b23
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890819"
---
# <a name="expeditedqualityupdatereference-resource-type"></a>Tipo de recurso expeditedQualityUpdateReference

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa Windows 10 conteúdo de atualização de qualidade para acelerar.

Em uma implantação, a mesma referência de atualização de qualidade acelerada pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.

Herda [de qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classificação|microsoft.graph.windowsUpdates.qualityUpdateClassification|Especifica a classificação do conteúdo referenciado. Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**. O valor padrão é `security`. Os valores possíveis são: `security` e `unknownFutureValue`. Herdado [de qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).|
|equivalentContent|microsoft.graph.windowsUpdates.equivalentContentOption|Especifica outro conteúdo a ser considerado como equivalente. Oferece suporte a um subconjunto dos valores **para equivalentContentOption**. O valor padrão é `latestSecurity`. Os valores possíveis são: `latestSecurity` e `unknownFutureValue`.|
|releaseDateTime|DateTimeOffset|Especifica uma atualização de qualidade com a **classificação** determinada por sua data de publicação (ou seja, a última atualização publicada na data especificada). Todos os dispositivos com uma atualização publicada antes da **versãoDateTime** receberão uma atualização de qualidade acelerada. Herdado [de qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)",
  "equivalentContent": "String"
}
```

