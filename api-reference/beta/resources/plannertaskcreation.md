---
title: Tipo de recurso plannerTaskCreation
description: Contém informações sobre a origem do plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8a2a4bf3aae5f23a04c7ecb8ad043631f946b20
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883228"
---
# <a name="plannertaskcreation-resource-type"></a>Tipo de recurso plannerTaskCreation

Namespace: microsoft.graph

Contém informações sobre a origem do [plannerTask](plannerTask.md). Esse recurso terá todas as suas propriedades definidas como ou exatamente uma propriedade terá um valor que indica que a tarefa foi criada pelo processo descrito `null` por essa propriedade. Todas as `null` propriedades indicam que essa tarefa não foi criada por nenhum processo especializado. Os aplicativos não precisam saber a origem da tarefa para poder trabalhar com ela; No entanto, alguns aplicativos podem usar as informações adicionais para fornecer experiências específicas em torno dessas tarefas. Consulte a documentação para recursos específicos para saber mais.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamsPublicationInfo|[plannerTeamsPublicationInfo](../resources/plannerteamspublicationinfo.md)|Informações sobre o processo de publicação que criou essa tarefa. `null` indica que a tarefa não foi criada por um processo de publicação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTaskCreation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskCreation",
  "teamsPublicationInfo": {
    "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
  }
}
```

