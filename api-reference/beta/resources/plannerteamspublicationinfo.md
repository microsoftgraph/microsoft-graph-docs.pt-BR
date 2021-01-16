---
title: Tipo de recurso plannerTeamsPublicationInfo
description: Contém informações detalhadas sobre o processo de publicação que criou um plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9db73bb5a914a848f3e19e079321681b22510e8e
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883227"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>Tipo de recurso plannerTeamsPublicationInfo

Namespace: microsoft.graph

Contém informações detalhadas sobre o processo de publicação que criou um [plannerTask](plannertask.md). Um processo de publicação cria cópias de tarefas com base em um modelo. Essas tarefas são criadas em vários planos e têm permissões restritas para os usuários; por exemplo, eles não podem ser excluídos e os usuários podem ser impedidos de editar determinados campos. A publicação é usada para distribuir tarefas em uma organização e acompanhar seu progresso centralmente.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que essa tarefa foi modificada pela última vez pelo processo de publicação. Somente leitura. |
|publicationId|String| O identificador da publicação. Somente leitura.|
|publishedToPlanId|String|O identificador do **plannerPlan** em que essa tarefa foi originalmente colocada. Somente leitura. |
|publishingTeamId|String| O identificador da equipe [que](team.md) iniciou o processo de publicação. Somente leitura.|
|publishingTeamName|String|O nome de exibição da equipe que iniciou o processo de publicação. Esse nome de exibição é apenas para referência e pode não representar o nome mais atualizado da equipe. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTeamsPublicationInfo",
  "publicationId": "String",
  "publishingTeamId": "String",
  "publishingTeamName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishedToPlanId": "String"
}
```

