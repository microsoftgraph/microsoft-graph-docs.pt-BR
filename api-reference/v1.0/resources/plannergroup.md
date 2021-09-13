---
title: Tipo de recurso plannerGroup
description: O **recurso plannerGroup** fornece acesso aos recursos do Planner para um grupo. Ele não contém propriedades usáveis.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1140d22b4b2f1bb5f863c19a741d08171c5f00f7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019255"
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

