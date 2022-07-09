---
title: Tipo de recurso accessReviewSet
description: Contêiner para os recursos base que expõem a API e os recursos de revisões de acesso. Atualmente, expõe apenas o recurso accessReviewScheduleDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a4310978c8c3578604523f9fa299581f5b24039a
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697971"
---
# <a name="accessreviewset-resource-type"></a>Tipo de recurso accessReviewSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para os recursos base que expõem a API e os recursos de revisões de acesso. Atualmente, expõe apenas a [relação accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

Herda de [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|Definições|[coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)| Representa o modelo e o agendamento para uma revisão de acesso. |
|historyDefinitions|[coleção accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)| Representa uma coleção de dados de histórico de revisão de acesso e os escopos usados para coletar esses dados.|

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

