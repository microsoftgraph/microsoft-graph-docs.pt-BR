---
title: tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5d19a1738d3369f2d910dd590062016acf3047ab
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950448"
---
# <a name="calendarpermission-resource-type"></a>tipo de recurso calendarPermission

As permissões de um usuário com quem o calendário é compartilhado. 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Leia as propriedades e os relacionamentos do objeto calendarPermission. |
| [Update](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Atualize o objeto calendarPermission. |
| [Delete](../api/calendarpermission-delete.md) | Nenhum | Exclua o objeto calendarPermission. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedRoles|coleção de cadeias de caracteres| Lista de níveis de permissão de compartilhamento permitidos para o calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Representa um compartilhamento que tem acesso ao calendário. Para o compartilhamento "minha organização", a propriedade **Address** é NULL. |
|id|Cadeia de caracteres| O identificador exclusivo do usuário (compartilhamento) com o qual o calendário foi compartilhado. Somente leitura.|
|isInsideOrganization|Booliano| True se o usuário em contexto (compartilhamento) estiver dentro da mesma organização que o proprietário do calendário.|
|isRemovable|Booliano| `True`Se o usuário puder ser removido da lista de compartilhamentos do calendário especificado, `false` caso contrário. O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado. Não é possível remover "minha organização" como um compartilhamento para um calendário.|
|role|calendarRoleType| Nível de permissão atual do compartilhamento de calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->