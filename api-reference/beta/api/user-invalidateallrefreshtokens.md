---
title: 'usuário: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como os cookies de sessão no navegador de um usuário), redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data e hora atual. Geralmente, essa operação é executada (por usuário ou um administrador), se o usuário tem um dispositivo perdido ou roubado.  Essa operação seria impedir o acesso a qualquer dado da organização acessado por meio de aplicativos no dispositivo sem que o usuário pela primeira vez, sendo necessário para entrar novamente. Na verdade, essa operação seria forçar o usuário entrar novamente para todos os aplicativos que eles tenham anteriormente consentiu, independente do dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c006787c0d68ae0c6ecbb331a9ff410f957a6f93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524524"
---
# <a name="user-invalidateallrefreshtokens"></a>usuário: invalidateAllRefreshTokens

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como os cookies de sessão no navegador de um usuário), redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data e hora atual. Geralmente, essa operação é executada (por usuário ou um administrador), se o usuário tem um dispositivo perdido ou roubado.  Essa operação seria impedir o acesso a qualquer dado da organização acessado por meio de aplicativos no dispositivo sem que o usuário pela primeira vez, sendo necessário para entrar novamente. Na verdade, essa operação seria forçar o usuário entrar novamente para todos os aplicativos que eles tenham anteriormente consentiu, independente do dispositivo.

Para os desenvolvedores, se o aplicativo tenta resgatar um token de acesso delegado para este usuário, usando um token invalidado refresh, o aplicativo receberá um erro. Se isso acontecer, o aplicativo será necessário adquirir um novo token refresh fazendo uma solicitação ao ponto de extremidade autorizar, que irá forçar o usuário entrar.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

+ Para um aplicativo permitir o assinadas no usuário para invalidar aplicativos eles tenham consentiu: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All
+ Para um aplicativo permitir que um administrador invalidar aplicativos um usuário aceitou: Directory.ReadWrite.All, Directory.AccessAsUser.All

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Esta operação não possui nenhum conteúdo de solicitação.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
