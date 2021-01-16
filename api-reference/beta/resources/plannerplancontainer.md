---
title: Tipo de recurso plannerPlanContainer
description: Representa um contêiner para um plannerPlan. O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8b3abb10892077159e6f02c33a31d501a75dba2a
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883225"
---
# <a name="plannerplancontainer-resource-type"></a>Tipo de recurso plannerPlanContainer

Namespace: microsoft.graph

Representa um contêiner para um [plannerPlan](plannerPlan.md). O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano. Isso significa que somente as pessoas autorizadas a trabalhar com o recurso que contém o plano poderão trabalhar com o plano e as tarefas dentro dele. Quando o recurso que contém é excluído, os planos contidos também são excluídos. As propriedades **de plannerPlanContainer** não podem ser alteradas depois que o plano é criado.

Atualmente, o Planner oferece suporte aos tipos de contêiner listados na tabela a seguir. Ao criar um plano, a **propriedade containerUrl** deve ser especificada com o caminho do recurso identificado na tabela.

|Tipo|Descrição|Caminho para o recurso|
|----|-----------|--------------------|
|group| O plano está contido em um grupo.| https://graph.microsoft.com/v1.0/groups/&lt;id&gt;|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|containerId|String|O identificador do recurso que contém o plano.|
|type|plannerContainerType| O tipo do recurso que contém o plano. Consulte a tabela anterior para ver os tipos com suporte. Os valores possíveis são: `group` e `unknownFutureValue`.|
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

