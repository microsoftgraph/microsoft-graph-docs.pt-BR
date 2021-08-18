---
title: Tipo de recurso plannerTeamsPublicationInfo
description: Contém informações detalhadas sobre o processo de publicação que criou um plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7cf298b4e9933e3019a72b0750cf01a95c2bf892609f3b601c0742eaf3b9e27d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244292"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>Tipo de recurso plannerTeamsPublicationInfo

Namespace: microsoft.graph

Contém informações detalhadas sobre o processo de publicação que criou um [plannerTask](plannertask.md). Um processo de publicação cria cópias de tarefas com base em um modelo. Essas tarefas são criadas em vários planos e têm permissões restritas para os usuários; por exemplo, eles não podem ser excluídos e os usuários podem ser impedidos de editar determinados campos. A publicação é usada para distribuir tarefas em uma organização e acompanhar seu progresso centralmente.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que essa tarefa foi modificada pela última vez pelo processo de publicação. Somente leitura. |
|publicationId|Cadeia de caracteres| O identificador da publicação. Somente leitura.|
|publishedToPlanId|Cadeia de caracteres|O identificador do **plannerPlan essa** tarefa foi originalmente colocada. Somente leitura. |
|publishingTeamId|Cadeia de caracteres| O identificador da equipe [que](team.md) iniciou o processo de publicação. Somente leitura.|
|publishingTeamName|Cadeia de caracteres|O nome de exibição da equipe que iniciou o processo de publicação. Esse nome de exibição é apenas para referência e pode não representar o nome mais atualizado da equipe. Somente leitura. |

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

