---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7aee071949fb5d7ded115f131e732b6d3626e6fd
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994831"
---
# <a name="update-calendarpermission"></a>Atualizar calendarPermission

Atualize as propriedades do objeto calendarPermission.

## <a name="permissions"></a>Permissões

Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Calendário | Delegado (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Aplicativo |
|:-----|:-----|:-----|:-----|
| calendário do usuário | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| calendário de grupo | Group.ReadWrite.All | Sem suporte. | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Atualizar as permissões especificadas do calendário principal de um usuário:
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

Atualizar as permissões especificadas de um calendário de Grupo:
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

Atualize as permissões especificadas do calendário do usuário que contém o evento identificado:
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|allowedRoles|coleção de cadeias de caracteres| Lista de níveis de permissão de compartilhamento permitidos para o calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](../resources/email.md)| Representa um compartilhamento que tem acesso ao calendário. Para o compartilhamento "minha organização", a propriedade **Address** é NULL. |
|id|String| O identificador exclusivo do usuário (compartilhamento) com o qual o calendário foi compartilhado. Somente leitura.|
|isInsideOrganization|Booliano| True se o usuário em contexto (compartilhamento) estiver dentro da mesma organização que o proprietário do calendário.|
|isRemovable|Booliano| `True`Se o usuário puder ser removido da lista de compartilhamentos do calendário especificado, `false` caso contrário. O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado. Não é possível remover "minha organização" como um compartilhamento para um calendário.|
|role|calendarRoleType| Nível de permissão atual do compartilhamento de calendário. Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
