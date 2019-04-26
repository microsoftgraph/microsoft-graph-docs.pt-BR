---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562944"
---
# <a name="schedulinggroup-resource-type"></a>tipo de recurso schedulingGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar schedulingGroup](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | Criar uma página `schedulingGroup`.|
|[Lista schedulingGroups](../api/schedule-list-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) conjunto | Obter uma lista dos `schedulingGroups` em um cronograma.|
|[Obter schedulingGroup](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | Obter um `schedulingGroup` por ID.|
|[Subtituir schedulingGroup](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | Substituir um `schedulingGroup`.|
|[Excluir schedulingGroup](../api/schedulinggroup-delete.md) | Nenhum | Marcar `schedulingGroup` como inativa.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |A ID da tarefa `schedulingGroup`.|
| Nome para exibição   | `string`      | O nome de exibição do grupo `schedulingGroup`. Obrigatório. |
| isActive          |`bool`      | Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes. Obrigatório. |
| userIds       | `collection(string)`    |  A lista de IDs é membro de usuários da `schedulingGroup`. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de hora em que isso `schedulingGroup` foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de hora em que isso `schedulingGroup` foi criado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedBy        |`microsoft.graph.identitySet`        |A identidade da última atualização `schedulingGroup`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
