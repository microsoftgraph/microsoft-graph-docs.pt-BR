---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 077acf9454a10612bd1f90d05e8c3042e80bd397
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154882"
---
# <a name="schedulinggroup-resource-type"></a>tipo de recurso schedulingGroup

Namespace: microsoft.graph

Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar](../api/schedule-list-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) conjunto | Obtenha a lista de **schedulingGroups** em um cronograma.|
|[Criar](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | Criar um nov **schedulingGroup**.|
|[Obter](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | Obtenha um **schedulingGroup** por ID.|
|[Delete](../api/schedulinggroup-delete.md) | Nenhum | Marque **schedulingGroup** como inativo.|
|[Substituir](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | Substituir **schedulingGroup**.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |ID do **schedulingGroup**.|
| displayName   | `string`      | O nome de exibição do**schedulingGroup**. Obrigatório. |
| isActive          |`bool`      | Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes. Obrigatório. |
| userIds       | `collection(string)`    |  A lista de IDs de usuários que são membros do**schedulingGroup**. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de hora em que esse **schedulingGroup** foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de hora em que esse **schedulingGroup** foi criado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedBy        | [identitySet](identityset.md) |A identidade da última atualização desse **schedulingGroup**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
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
  "suppressions": []
}
-->
