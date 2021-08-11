---
title: Tipo de recurso calendarPermission
description: As permissões de um usuário com o qual o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 537055ca9f5ec1166d7c85f9d6a172384f564571e77a04c53c5a1c6d9331fc69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155187"
---
# <a name="calendarpermission-resource-type"></a>Tipo de recurso calendarPermission

As permissões de um usuário com o qual o calendário foi compartilhado ou delegado em um Outlook cliente.

Obter, atualizar e excluir permissões de calendário é suportado em nome apenas do proprietário do calendário.

Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.

Depois que um compartilhamento ou representante for definido [](../api/calendarpermission-update.md) para um calendário, você poderá atualizar apenas a propriedade **role** para alterar as permissões de um compartilhamento ou representante. Não é **possível atualizar** a **propriedade allowedRoles**, **emailAddress**, **isInsideOrganization** ou **isRemovable.** Para alterar essas propriedades, [exclua](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e crie outro compartilhamento ou representante em um cliente Outlook cliente.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Ler propriedades e relações do objeto calendarPermission. |
| [Atualizar](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Atualizar objeto calendarPermission. |
| [Delete](../api/calendarpermission-delete.md) | None | Excluir objeto calendarPermission. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedRoles|[Coleção calendarRoleType](#calendarroletype-values)| Lista de níveis de permissão de compartilhamento ou delegação permitidos para o calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Representa um compartilhamento ou representante que tem acesso ao calendário. Para o compartilhamento "Minha Organização", a propriedade **address** é nula. Somente leitura. |
|id|Cadeia de caracteres| O identificador exclusivo do usuário (compartilhamento ou representante) com o qual o calendário foi compartilhado. Apenas leitura.|
|isInsideOrganization|Booliano| True se o usuário no contexto (compartilhamento ou representante) estiver dentro da mesma organização que o proprietário do calendário.|
|isRemovable|Booliano| `True` se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário. O usuário "Minha organização" determina as permissões que outras pessoas em sua organização têm para o calendário determinado. Não é possível remover "Minha organização" como um compartilhamento para um calendário.|
|role|[calendarRoleType](#calendarroletype-values)| Nível de permissão atual do compartilhamento de calendário ou representante. |

### <a name="calendarroletype-values"></a>Valores calendarRoleType

| Member        | Descrição |
|:--------------|:------------|
| nenhuma | Calendário não é compartilhado com o usuário. |
| freeBusyRead | O usuário é um compartilhamento que pode exibir o status de livre/ocupado do proprietário no calendário. |
| limitedRead | O usuário é um compartilhamento que pode exibir o status de livre/ocupado e títulos e locais dos eventos no calendário. |
| leitura | O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos particulares do proprietário. |
| gravação | O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos particulares) e editar eventos no calendário. |
| delegateWithoutPrivateEventAccess | O usuário é um representante que tem acesso a gravação, mas não pode exibir informações dos eventos privados do proprietário no calendário. |
| delegateWithPrivateEventAccess | O usuário é um representante que tem acesso a gravação e pode exibir informações dos eventos privados do proprietário no calendário. |
| custom | O usuário tem permissões personalizadas para o calendário. |


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
