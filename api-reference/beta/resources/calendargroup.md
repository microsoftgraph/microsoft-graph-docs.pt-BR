---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 89a0a8176936654e287399c51c45e9ae55f46f23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071616"
---
# <a name="calendargroup-resource-type"></a>Tipo de recurso calendarGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de calendários do usuário.

## <a name="methods"></a>Métodos

| Método                                                      | Tipo de retorno                        | Descrição                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [List calendar groups](../api/user-list-calendargroups.md)  | Coleção [Calendar](calendar.md) | Obter os grupos de calendários do usuário.                               |
| [Create calendar group](../api/user-post-calendargroups.md) | [Calendar](calendar.md)            | Criar um novo grupo de calendários.                                  |
| [Get calendar group](../api/calendargroup-get.md)           | [calendarGroup](calendargroup.md)  | Leia as propriedades e os relacionamentos de um objeto de grupo de calendários. |
| [Update](../api/calendargroup-update.md)                    | [calendarGroup](calendargroup.md)  | Atualize o objeto calendarGroup.                                  |
| [Delete](../api/calendargroup-delete.md)                    | Nenhum                               | Exclua o objeto calendarGroup.                                  |
| [Listar calendários](../api/calendargroup-list-calendars.md)    | Coleção [Calendar](calendar.md) | Liste os calendários em um grupo de calendários.                           |
| [Create Calendar](../api/calendargroup-post-calendars.md)   | [Calendar](calendar.md)            | Crie um novo calendário em um grupo de calendários.                    |

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| name      | Cadeia de caracteres | O nome do grupo.                                                                                                                                                                                           |
| changeKey | Cadeia de caracteres | Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura. |
| classId   | Guid   | O identificador de classe. Somente leitura.                                                                                                                                                                          |
| id        | String | O identificador exclusivo do grupo. Somente leitura.                                                                                                                                                                 |

## <a name="relationships"></a>Relacionamentos

| Relação | Tipo                               | Descrição                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| calendars    | Coleção [Calendar](calendar.md) | Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
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

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


