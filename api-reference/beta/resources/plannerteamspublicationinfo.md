---
title: Tipo de recurso plannerTeamsPublicationInfo
description: Contém informações detalhadas sobre o processo de publicação que criou um plannerTask.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 77441184468a87e6d12d32adedc98a26c228db68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115041"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>Tipo de recurso plannerTeamsPublicationInfo

Namespace: microsoft.graph

Contém informações detalhadas sobre o processo de publicação que criou um [plannerTask](plannertask.md). Um processo de publicação cria cópias de tarefas com base em um modelo. Essas tarefas são criadas em vários planos e têm permissões restritas para os usuários; por exemplo, eles não podem ser excluídos e os usuários podem ser impedidos de editar determinados campos. A publicação é usada para distribuir tarefas em uma organização e acompanhar seu progresso centralmente.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que essa tarefa foi modificada pela última vez pelo processo de publicação. Somente leitura. |
|publicationId|Cadeia de Caracteres| O identificador da publicação. Somente leitura.|
|publishedToPlanId|Cadeia de Caracteres|O identificador do **plannerPlan essa** tarefa foi originalmente colocada. Somente leitura. |
|publishingTeamId|Cadeia de Caracteres| O identificador da equipe [que](team.md) iniciou o processo de publicação. Somente leitura.|
|publishingTeamName|Cadeia de Caracteres|O nome de exibição da equipe que iniciou o processo de publicação. Esse nome de exibição é apenas para referência e pode não representar o nome mais atualizado da equipe. Somente leitura. |

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

