---
title: Tipo de recurso plannerGroup
description: O **recurso plannerGroup** fornece acesso aos recursos do Planner para um grupo. Ele não contém propriedades usáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: be82fb6988c88f40bc975af28240e9a99f6f9d5c13ec7069af93c3f34b92e04c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205224"
---
# <a name="plannergroup-resource-type"></a>Tipo de recurso plannerGroup

Namespace: microsoft.graph

O **recurso plannerGroup** fornece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém propriedades usáveis.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar planos](../api/plannergroup-list-plans.md) |coleção [plannerPlan](plannerplan.md)| Obter uma **coleção de objetos plannerPlan.**|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. Identificador do **plannerGroup**|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|plans|coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna os [plannerPlans pertencentes](plannerplan.md) ao grupo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

