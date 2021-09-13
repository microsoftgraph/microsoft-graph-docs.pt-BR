---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários de usuários.
author: harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ca67a29dd6c48119442423570a08b66dd5a83f9b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129961"
---
# <a name="calendargroup-resource-type"></a>Tipo de recurso calendarGroup

Namespace: microsoft.graph

Um grupo de calendários de usuários.

## <a name="methods"></a>Métodos

| Método                                                      | Tipo de retorno                        | Descrição                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [List calendar groups](../api/user-list-calendargroups.md)  | Coleção [Calendar](calendar.md) | Obter os grupos de calendários do usuário.                               |
| [Create calendar group](../api/user-post-calendargroups.md) | [Calendar](calendar.md)            | Criar um novo grupo de calendários.                                  |
| [Get calendar group](../api/calendargroup-get.md)           | [calendarGroup](calendargroup.md)  | Leia as propriedades e os relacionamentos de um objeto de grupo de calendários. |
| [Update](../api/calendargroup-update.md)                    | [calendarGroup](calendargroup.md)  | Atualize o objeto calendarGroup.                                  |
| [Delete](../api/calendargroup-delete.md)                    | Nenhum(a)                               | Exclua o objeto calendarGroup.                                  |
| [Listar calendários](../api/calendargroup-list-calendars.md)    | Coleção [Calendar](calendar.md) | Liste os calendários em um grupo de calendários.                           |
| [Create Calendar](../api/calendargroup-post-calendars.md)   | [Calendar](calendar.md)            | Crie um novo calendário em um grupo de calendários.                    |

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| nome      | String | O nome do grupo.                                                                                                                                                                                           |
| changeKey | String | Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura. |
| classId   | Guid   | O identificador de classe. Somente leitura.                                                                                                                                                                          |
| id        | String | O identificador exclusivo do grupo. Somente leitura.                                                                                                                                                                 |

## <a name="relationships"></a>Relações

| Relação | Tipo                               | Descrição                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| calendars    | Coleção [Calendar](calendar.md) | Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

