---
title: Tipo de recurso plannerTaskCreation
description: Contém informações sobre a origem do plannerTask.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 49d1ec116108cb955c353c00e59b34efe534694a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125586"
---
# <a name="plannertaskcreation-resource-type"></a>Tipo de recurso plannerTaskCreation

Namespace: microsoft.graph

Contém informações sobre a origem do [plannerTask](plannerTask.md). Esse recurso terá todas as suas propriedades definidas como , ou exatamente uma propriedade terá um valor que indica que a tarefa foi criada pelo processo descrito `null` por essa propriedade. Todas as `null` propriedades indicam que essa tarefa não foi criada por nenhum processo especializado. Os aplicativos não precisam saber a origem da tarefa para poder trabalhar com ela; no entanto, alguns aplicativos podem usar as informações adicionais para fornecer experiências específicas em torno dessas tarefas. Consulte a documentação para saber mais sobre recursos específicos.

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

