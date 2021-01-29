---
title: Excluir windowsHelloForBusinessAuthenticationMethod
description: Exclui um objeto windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b75a5c106aed98bfab00f2e4832a6c1d1ab598d
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052542"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a>Excluir windowsHelloForBusinessAuthenticationMethod
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Permissões agindo por si só

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

### <a name="permissions-acting-on-other-users"></a>Permissões atuando em outros usuários

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | UserAuthenticationMethod.ReadWrite.All |

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Administração global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

