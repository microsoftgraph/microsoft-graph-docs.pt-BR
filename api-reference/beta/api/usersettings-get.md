---
title: Obter configurações
description: Leia o usuário e o objeto de configurações da organização.
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 309e27bd0cc197347ebd87aec6d1a968586ab167
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60935155"
---
# <a name="get-settings"></a>Obter configurações

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia o objeto [userSettings](../resources/usersettings.md) do usuário e da organização. Para saber como atualizar as propriedades do objeto [userSettings](../resources/usersettings.md), consulte [atualizar as configurações do usuário](usersettings-update.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read.All, User.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
GET /me/settings/
```

A solicitação com uma 'ID de usuário' ou 'userPrincipalName' só pode ser acessada pelo usuário ou por um usuário com as permissões User.ReadWrite.All. Para saber mais, consulte [Permissões](/graph/permissions-reference).

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [userSettings](../resources/usersettings.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a>Resposta

Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```


