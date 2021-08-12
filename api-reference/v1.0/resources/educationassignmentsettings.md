---
title: Tipo de recurso educationAssignmentSettings
description: Especifica as configurações de atribuições de nível de classe.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c920db8b8d3b6ea8a3c49e4a4816740d59a8e534aa542a1a906451654eaf7f6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212106"
---
# <a name="educationassignmentsettings-resource-type"></a>Tipo de recurso educationAssignmentSettings

Namespace: microsoft.graph

Especifica as configurações de atribuições de nível de classe.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)|
|[Atualizar educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Atualize as propriedades de [um objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|submissionAnimationDisabled|Booliano|Indica se a animação de celebração de turn-in será mostrada. Um valor `true` indica que a animação não será mostrada. O valor padrão é `false`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

