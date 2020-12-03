---
title: Instalar o aplicativo para o usuário
description: Instale um aplicativo no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 984157470aeceb019e234aa11c3bd693bcc6b9b0
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564015"
---
# <a name="install-app-for-user"></a>Instalar o aplicativo para o usuário

Namespace: microsoft.graph

Instalar um [aplicativo](../resources/teamsapp.md) no escopo pessoal do [usuário](../resources/user.md)especificado.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | TeamsAppInstallation. ReadWriteSelfForUser, TeamsAppInstallation. ReadWriteForUser, TeamsAppInstallation. ReadWrite |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All, TeamsAppInstallation. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação deve conter a ID do aplicativo de catálogo existente a ser adicionado.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|teamsApp|String|A ID do aplicativo a ser adicionado.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->

```http
POST https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
