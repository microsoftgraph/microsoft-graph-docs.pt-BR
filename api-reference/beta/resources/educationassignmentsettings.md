---
title: Tipo de recurso educationAssignmentSettings
description: Especifica configurações de atribuições de nível de classe.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c670cb2bbef0b82ff80996e4acb52c2826ec118f
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034325"
---
# <a name="educationassignmentsettings-resource-type"></a>Tipo de recurso educationAssignmentSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica configurações de atribuições de nível de classe.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Leia as propriedades e os relacionamentos de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)|
|[Atualizar educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Atualizar as propriedades de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|submissionAnimationDisabled|Boolean|Indica se a animação de celebração de turn-in será mostrada. Um valor indica `true` que a animação não será mostrada. O valor padrão é `false`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

