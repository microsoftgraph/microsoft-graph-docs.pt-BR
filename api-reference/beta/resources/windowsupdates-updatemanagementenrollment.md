---
title: Tipo de recurso updateManagementEnrollment
description: Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d00bc152d5fc3b7b4be267cd3ea56fab52b8b38
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067232"
---
# <a name="updatemanagementenrollment-resource-type"></a>Tipo de recurso updateManagementEnrollment

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.

Herda [de updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|A categoria de atualizações que o serviço gerencia. Oferece suporte a um subconjunto dos valores **para updateCategory**. Os valores possíveis são: `feature` .|

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

