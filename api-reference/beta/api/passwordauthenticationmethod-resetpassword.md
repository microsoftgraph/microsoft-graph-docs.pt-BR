---
title: 'passwordAuthenticationMethod: resetPassword'
description: Redefinir a senha de um usuário
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3e07320950184a89c9d8000145b75af978a4e1e1
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646582"
---
# <a name="passwordauthenticationmethod-resetpassword"></a>passwordAuthenticationMethod: resetPassword

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inicie uma redefinição da senha associada a um objeto [de método de autenticação de](../resources/passwordauthenticationmethod.md) senha. Isso só pode ser feito por um administrador com permissões apropriadas e não pode ser executado na conta de um usuário.

Esse fluxo grava a nova senha para Azure Active Directory e a pressiona para Active Directory local configurada usando writeback de senha. O administrador pode fornecer uma nova senha ou fazer com que o sistema gere uma. O usuário é solicitado a alterar a senha na próxima vez que entrar.

Essa redefinição é uma operação de longa duração e retornará um header **Location** com um link onde o chamador pode verificar periodicamente o status da operação de redefinição.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

> [!IMPORTANT]
> A operação não pode ser executada na conta de um usuário. Somente um administrador com as permissões apropriadas pode executar essa operação.

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegado (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes funções [do Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
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
|newPassword|Cadeia de caracteres|A nova senha. Obrigatório para locatários com cenários de senha híbrida. Se for omitido para uma senha somente na nuvem, o sistema retornará uma senha gerada pelo sistema. Esta é uma cadeia de caracteres unicode sem outra codificação. Ele é validado no sistema de senhas proibido do locatário antes da aceitação e deve seguir os requisitos de senha na nuvem e/ou local do locatário.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um header **location** com uma URL para verificar o status da operação de redefinição.

Se o chamador não enviar uma senha, uma senha gerada pela Microsoft será fornecida em um objeto JSON no corpo da resposta.

### <a name="response-headers"></a>Cabeçalhos de resposta

| Nome        | Descrição     |
|:------------|:----------------|
|Local     | URL a ser chamada para verificar o status da operação. Obrigatório.|
|Repetir-after  | Duração em segundos. Opcional.|

## <a name="examples"></a>Exemplos

### <a name="example-1-user-submitted-password"></a>Exemplo 1: senha enviada pelo usuário

O exemplo a seguir mostra como chamar essa API quando o chamador envia uma senha.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-type: application/json

{
    "newPassword": "Cuyo5459"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-adminprovided-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/operations/88e7560c-9ebf-435c-8089-c3998ac1ec51?aadgdc=DUB02P&aadgsu=ssprprod-a

{}
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

O exemplo a seguir mostra como chamar essa API quando o chamador não envia uma senha.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-systemgenerated-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/operations/77bafe36-3ac0-4f89-96e4-a4a5a48da851?aadgdc=DUB02P&aadgsu=ssprprod-a
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.passwordResetResponse",
    "newPassword": "Cuyo5459"
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
