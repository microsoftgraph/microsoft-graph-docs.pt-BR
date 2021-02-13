---
title: Tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8162220df0ebf6973f1b317c1e4c063dbc98de3e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176700"
---
# <a name="calendarpermission-resource-type"></a>Tipo de recurso calendarPermission

As permissões de um usuário com o qual o calendário foi compartilhado ou delegado em um cliente do Outlook.

Obter, atualizar e excluir permissões de calendário é suportado em nome apenas do proprietário do calendário.

Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.

Depois que um compartilhamento ou representante tiver sido [](../api/calendarpermission-update.md) definido  para um calendário, você poderá atualizar apenas a propriedade de função para alterar as permissões de um compartilhamento ou representante. Você não **pode atualizar** a **propriedade allowedRoles**, **emailAddress**, **isInsideOrganization** ou **isRemovable.** Para alterar essas propriedades, você deve [excluir](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e criar outro compartilhamento ou representante em um cliente do Outlook.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Leia as propriedades e os relacionamentos do objeto calendarPermission. |
| [Update](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Atualize o objeto calendarPermission. |
| [Delete](../api/calendarpermission-delete.md) | Nenhum | Exclua o objeto calendarPermission. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedRoles|[Coleção calendarRoleType](#calendarroletype-values)| Lista de níveis de permissão permitidos de compartilhamento ou de delegação do calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Representa um compartilhamento ou representante que tem acesso ao calendário. Para o compartilhamento "Minha Organização", a propriedade **de** endereço é nula. Somente leitura. |
|id|Cadeia de caracteres| O identificador exclusivo do usuário (compartilhar ou delegar) com quem o calendário foi compartilhado. Somente leitura.|
|isInsideOrganization|Boolean| True se o usuário no contexto (compartilhar ou delegar) estiver dentro da mesma organização que o proprietário do calendário.|
|isRemovable|Booliano| `True` se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário. O usuário "Minha organização" determina as permissões que outras pessoas em sua organização têm para o calendário determinado. Não é possível remover "Minha organização" como um compartilhamento de um calendário.|
|role|[calendarRoleType](#calendarroletype-values)| Nível de permissão atual do compartilhamento de calendário ou representante. |

### <a name="calendarroletype-values"></a>Valores de calendarRoleType

| Member        | Descrição |
|:--------------|:------------|
| nenhum | O calendário não é compartilhado com o usuário. |
| freeBusyRead | O usuário é um compartilhamento que pode exibir o status de livre/ocupado do proprietário no calendário. |
| limitedRead | O usuário é um compartilhamento que pode exibir o status de livre/ocupado e títulos e locais dos eventos no calendário. |
| leitura | O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos particulares do proprietário. |
| gravação | O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos privados) e editar eventos no calendário. |
| delegateWithoutPrivateEventAccess | O usuário é um representante que tem acesso de gravação, mas não pode exibir informações dos eventos particulares do proprietário no calendário. |
| delegateWithPrivateEventAccess | O usuário é um representante que tem acesso de gravação e pode exibir informações dos eventos particulares do proprietário no calendário. |
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
