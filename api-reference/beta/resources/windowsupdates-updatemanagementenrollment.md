---
title: Tipo de recurso updateManagementEnrollment
description: Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8d780894e90a1f6eec748a9f62f486b39d3c6cfb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890182"
---
# <a name="updatemanagementenrollment-resource-type"></a>Tipo de recurso updateManagementEnrollment

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.

Herda [de updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|A categoria de atualizações que o serviço gerencia. Oferece suporte a um subconjunto dos valores **para updateCategory**. Os valores possíveis são: `feature`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updateManagementEnrollment",
  "updateCategory": "String"
}
```

