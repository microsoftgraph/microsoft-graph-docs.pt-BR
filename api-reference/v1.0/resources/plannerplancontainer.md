---
title: tipo de recurso plannerPlanContainer
description: Representa um contêiner para um plannerPlan. O contêiner é um recurso que especifica as regras de autorização e a duração do plano.
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: dbb95f1124461e12b36d6c4f69dac193aa349b15
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420780"
---
# <a name="plannerplancontainer-resource-type"></a>tipo de recurso plannerPlanContainer

Namespace: microsoft.graph

Representa um contêiner para um [plannerPlan](plannerplan.md). O contêiner é um recurso que especifica as regras de autorização e a duração do plano. Isto significa que somente as pessoas que são autorizadas a trabalhar com o recurso que contém o plano poderão trabalhar com o plano e as tarefas dentro dele. Quando o recurso contido é excluído, os planos contidos também são excluídos. As propriedades do **plannerPlanContainer** não podem ser alteradas depois que o plano é criado.

O Microsoft Planner atualmente dá suporte aos tipos de contêiner listados na tabela a seguir. Ao criar um plano, você deve especificar a propriedade **containerUrl** com o caminho do recurso identificado na tabela a seguir.

|Tipo|Descrição|Caminho para o recurso|
|----|-----------|--------------------|
|group| O plano está contido por um [grupo](group.md).| https://graph.microsoft.com/v1.0/groups/{id}|
|lista de participantes| O plano está contido por um **plannerRoster** | https://graph.microsoft.com/beta/planner/rosters/{id}. Atualmente, os **PlannerRosters** só são acessíveis usando a versão beta.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|containerId|Cadeia de caracteres|O identificador do recurso que contém o plano.|
|type|plannerContainerType| O tipo do recurso que contém o plano. Para tipos com suporte, consulte a tabela anterior. Os valores possíveis são: `group`, `unknownFutureValue`, `roster`. Observe que você deve usar o cabeçalho de `Prefer: include-unknown-enum-members` solicitação para obter o seguinte valor nessa [enumeração evolutiva](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `roster`.|
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
  "containerId": "String",
  "type": "String",
  "url": "String"
}
```

