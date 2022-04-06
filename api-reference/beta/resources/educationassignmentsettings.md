---
title: Tipo de recurso educationAssignmentSettings
description: Especifica as configurações de atribuições de nível de classe.
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fe1a8cf70f717df396bf8b336f3a543770a4da71
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684876"
---
# <a name="educationassignmentsettings-resource-type"></a>Tipo de recurso educationAssignmentSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica as configurações de atribuições de nível de classe.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Leia as propriedades e as relações de um [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) .|
|[Atualizar educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Atualize as propriedades de [um objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para educationAssignmentSettings.|
|submissionAnimationDisabled|Booliano|Indica se a animação de celebração de entrega será mostrada. Um valor de `true` indica que a animação não será mostrada. O valor padrão é `false`.|

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
  "id": "String (identifier)",
  "submissionAnimationDisabled": false
}
```

