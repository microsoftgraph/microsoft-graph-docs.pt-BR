---
title: Tipo de recurso updateManagementEnrollment
description: Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 992cfc8ebf53db3b1f3aad7c3c997d02344a503b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861580"
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

