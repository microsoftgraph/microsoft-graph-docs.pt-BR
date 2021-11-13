---
title: Tipo de recurso deploymentStateReason
description: Um motivo para um estado de implantação específico.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 54240d057734d17df3e0df3a270d1aab00022586
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890448"
---
# <a name="deploymentstatereason-resource-type"></a>Tipo de recurso deploymentStateReason

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um motivo para um estado de implantação específico.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|valor|microsoft.graph.windowsUpdates.deploymentStateReasonValue|Especifica um motivo para o estado de implantação. Os valores possíveis são: `scheduledByOfferWindow`, `offeringByRequest`, `pausedByRequest`, `pausedByMonitoring`. Observe que você deve usar o header de solicitação para obter os seguintes valores nesta `Prefer: include-unknown-enum-members` [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `faultedByContentOutdated` . Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentStateReason",
  "value": "String"
}
```

