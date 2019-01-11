---
title: Obter configurações
description: Leia o objeto de configurações de usuário e da organização.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: ace7c43b27860832968572628838484bc8c91c84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815488"
---
# <a name="get-settings"></a>Obter configurações

Leia o objeto de [configurações](../resources/user-settings.md) de usuário e da organização.
Para saber como atualizar as propriedades do objeto de [configurações](../resources/user-settings.md) , consulte [Atualizar configurações de usuário](user-update-settings.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read.All, User.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
GET /me/settings/
```

Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário ou por um usuário com as permissões User.ReadWrite.All. Para saber mais, consulte [Permissions](/graph/permissions-reference).

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` objeto de [configurações de usuário](../resources/user-settings.md) e o código de resposta no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/me/settings
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

