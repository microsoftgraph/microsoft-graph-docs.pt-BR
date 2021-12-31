---
title: Tipo de recurso accessReviewSet
description: Contêiner para os recursos base que expõem a API e os recursos de críticas de acesso. Atualmente, expõe apenas o recurso accessReviewScheduleDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f1d3b28da541a365d1507cefce8d18adbc407dae
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650774"
---
# <a name="accessreviewset-resource-type"></a>Tipo de recurso accessReviewSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para os recursos base que expõem a API e os recursos de críticas de acesso. Atualmente, expõe apenas a relação [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|definições|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)| Representa o modelo e o agendamento para uma revisão de acesso. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewSet"
}
```

