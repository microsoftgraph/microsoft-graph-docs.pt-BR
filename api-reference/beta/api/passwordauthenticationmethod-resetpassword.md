---
title: 'passwordAuthenticationMethod: resetPassword'
description: Redefinir a senha de um usuário
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5e2544e0f9a7e5bc0530aa4585deb613274a9041
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557805"
---
# <a name="passwordauthenticationmethod-resetpassword"></a>passwordAuthenticationMethod: resetPassword

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inicie uma redefinição para a senha associada a um objeto de [método de autenticação de senha](../resources/passwordauthenticationmethod.md) . Isso só pode ser feito por um administrador com as permissões apropriadas e não pode ser executado na conta de um usuário.

Este fluxo grava a nova senha no Azure Active Directory e a envia para o Active Directory local, se configurado usando o Write-back de senha. O administrador pode fornecer uma nova senha ou fazer com que o sistema gere uma. O usuário é solicitado a alterar a senha na próxima vez em que entrar.

Essa redefinição é uma operação de execução longa e retornará um link no `Location` cabeçalho onde o chamador pode verificar periodicamente o status da redefinição.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões que atuam em si (de menos para mais privilégios) | Permissões que atuam em outros (de menos para mais privilégios)|
|:---------------------------------------|:-------------------------|:-----------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All | UserAuthenticationMethod. ReadWrite. All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. | Sem suporte. |
| Aplicativo                            | Sem suporte. | Sem suporte. |

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|newPassword|String|A nova senha inserida pelo administrador. Obrigatório para locatários com cenários de senha híbrida. Se for omitido para uma senha somente de nuvem, o sistema retornará uma senha gerada pelo sistema. Esta é uma cadeia de caracteres Unicode sem codificação. Ele é validado em relação ao sistema de senha banida do locatário antes da aceitação e deve cumprir a nuvem do locatário e/ou os requisitos de senha local.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `202 ACCEPTED` um código de resposta e uma URL `Location` no cabeçalho.

Se o chamador não enviar uma senha, uma senha gerada pela Microsoft será fornecida em um objeto JSON no corpo da resposta.

### <a name="response-headers"></a>Cabeçalhos de resposta

| Nome        | Descrição     |
|:------------|:----------------|
|Local     | URL a ser chamada para verificar o status da operação.|
|Repetir-após  | Duração em segundos.|

## <a name="examples"></a>Exemplos

### <a name="example-1-user-submitted-password"></a>Exemplo 1: senha enviada pelo usuário

O exemplo a seguir mostra como chamar essa API quando o chamador enviar uma senha.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/authentication/passwordMethods/{id}/resetPassword
Content-type: application/json

{
  "newPassword": "newPassword-value",
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 ACCEPTED
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/{id}/authentication/operations/{id}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-system-generated-password"></a>Exemplo 2: senha gerada pelo sistema

O exemplo a seguir mostra como chamar essa API quando o chamador não enviar uma senha.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/authentication/passwordMethods/{id}/resetPassword
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/{id}/authentication/operations/{id}
Content-type: application/json

{
  "password": "new system generated password"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
