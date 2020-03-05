---
title: tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c038ccd69cefa66c4fd57f4b09273662320f2640
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507835"
---
# <a name="calendarpermission-resource-type"></a>tipo de recurso calendarPermission

Namespace: Microsoft. Graph

As permissões de um usuário com o qual o calendário foi compartilhado ou delegado em um cliente do Outlook.

Obter, atualizar e excluir permissões de calendário é suportada em nome apenas do proprietário do calendário.

Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.

Depois que um compartilhamento ou representante tiver sido configurado para um calendário, você poderá [Atualizar](../api/calendarpermission-update.md) somente a propriedade **role** para alterar as permissões de um compartilhamento ou representante. Não é possível **Atualizar** a propriedade **allowedRoles**, **EmailAddress**, **isInsideOrganization**ou **isRemovable** . Para alterar essas propriedades, você deve [excluir](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e criar outro compartilhamento ou representante em um cliente do Outlook.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Leia as propriedades e os relacionamentos do objeto calendarPermission. |
| [Update](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Atualize o objeto calendarPermission. |
| [Delete](../api/calendarpermission-delete.md) | Nenhum | Exclua o objeto calendarPermission. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedRoles|coleção [calendarRoleType](#calendarroletype-values)| Lista de níveis de permissão de compartilhamento ou de delegação permitidos para o calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Representa um compartilhamento ou representante que tem acesso ao calendário. Para o compartilhamento "minha organização", a propriedade **Address** é NULL. Somente leitura. |
|id|String| O identificador exclusivo do usuário (compartilhamento ou representante) com o qual o calendário foi compartilhado. Somente leitura.|
|isInsideOrganization|Boolean| True se o usuário em contexto (compartilhamento ou representante) estiver dentro da mesma organização que o proprietário do calendário.|
|isRemovable|Booliano| `True`Se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário. O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado. Não é possível remover "minha organização" como um compartilhamento para um calendário.|
|role|[calendarRoleType](#calendarroletype-values)| Nível de permissão atual do compartilhamento ou representante do calendário. |

### <a name="calendarroletype-values"></a>valores de calendarRoleType

| Valores        | Descrição |
|:--------------|:------------|
| nenhuma | O calendário não é compartilhado com o usuário. |
| freeBusyRead | O usuário é um compartilhamento que pode exibir o status de disponibilidade do proprietário no calendário. |
| limitedRead | O usuário é um compartilhamento que pode exibir o status de disponibilidade e os títulos e locais dos eventos no calendário. |
| Saiba | O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos privados do proprietário. |
| gravável | O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos privados) e editar eventos no calendário. |
| delegateWithoutPrivateEventAccess | O usuário é um representante que tem acesso de gravação, mas não pode exibir informações dos eventos privados do proprietário no calendário. |
| delegateWithPrivateEventAccess | O usuário é um representante que tem acesso de gravação e pode exibir informações dos eventos privados do proprietário no calendário. |
| cliente | O usuário tem permissões personalizadas para o calendário. |


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