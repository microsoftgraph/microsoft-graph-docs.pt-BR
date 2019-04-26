---
title: Obter configurações
description: Leia o objeto de configurações de organização e usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dcd9079956b4db8b349ba6b81bd85d8472630643
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334903"
---
# <a name="get-settings"></a>Obter configurações

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia o objeto de [configurações](../resources/user-settings.md) de organização e usuário.
Para saber como atualizar as propriedades do objeto de [configurações](../resources/user-settings.md) , consulte [Update User Settings](user-update-settings.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read.All, User.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User. Read. All, User. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

```http
GET /me/settings/
```

A solicitação com uma "ID de usuário" ou "userPrincipalName" só pode ser acessada pelo usuário ou por um usuário com as permissões User. ReadWrite. All. Para saber mais, confira [permissões](/graph/permissions-reference).

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de [configurações do usuário](../resources/user-settings.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
