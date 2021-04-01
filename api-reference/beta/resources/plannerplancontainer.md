---
title: Tipo de recurso plannerPlanContainer
description: Representa um contêiner para um plannerPlan. O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: acb7a85683bc94795953e524ee9630d6cfc01f24
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473882"
---
# <a name="plannerplancontainer-resource-type"></a>Tipo de recurso plannerPlanContainer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para um [plannerPlan](plannerPlan.md). O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano. Isso significa que somente as pessoas que estão autorizadas a trabalhar com o recurso que contém o plano poderão trabalhar com o plano e as tarefas dentro dele. Quando o recurso que contém é excluído, os planos contidos também são excluídos. As propriedades **do plannerPlanContainer** não podem ser alteradas após a criação do plano.

No momento, o Planner dá suporte aos tipos de contêiner listados na tabela a seguir. Ao criar um plano, a **propriedade containerUrl** deve ser especificada com o caminho do recurso identificado na tabela.

|Tipo|Descrição|Caminho para o recurso|
|----|-----------|--------------------|
|group| O plano está contido em um [grupo](group.md).| https://graph.microsoft.com/beta/groups/&lt;id&gt;|
|roster| O plano está contido por [um plannerRoster](plannerroster.md) | https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|containerId|String|O identificador do recurso que contém o plano.|
|tipo|plannerContainerType| O tipo do recurso que contém o plano. Consulte a tabela anterior para tipos com suporte. Os valores possíveis são: `group`, `roster`, `unknownFutureValue`.|
|url|Cadeia de caracteres|A URL canônica completa do contêiner.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "url": "String",
  "containerId": "String",
  "type": "String"
}
```

