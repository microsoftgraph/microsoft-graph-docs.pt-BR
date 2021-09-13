---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: akumar39
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 998bd2ed3cf05db84dd17c4ef6c166474721105d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035959"
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
| displayName   | `string`      | O nome de exibição do **schedulingGroup**. Necessário. |
| isActive          |`bool`      | Indica se o `schedulingGroup` pode ser usado na criação de novas entidades ou atualizar as existentes. Necessário. |
| userIds       | `collection(string)`    |  A lista de IDs de usuário que são membros do **schedulingGroup**. Necessário. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora no qual este **schedulingGroup** foi criado pela primeira vez. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/hora no qual este **schedulingGroup** foi atualizado pela última vez. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
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

