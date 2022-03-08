---
title: Tipo de recurso accessReviewSet
description: Contêiner para os recursos base que expõem a API e os recursos de críticas de acesso. Atualmente, expõe apenas o recurso accessReviewScheduleDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4964b26b1f6c415a0e822c6d47e67499876011b1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333215"
---
# <a name="accessreviewset-resource-type"></a>Tipo de recurso accessReviewSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para os recursos base que expõem a API e os recursos de críticas de acesso. Atualmente, expõe apenas a relação [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|definições|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)| Representa o modelo e o agendamento para uma revisão de acesso. |
|historyDefinitions|[Coleção accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)| Representa uma coleção de dados de histórico de revisão de acesso e os escopos usados para coletar esses dados.|

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

