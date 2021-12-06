---
title: Criar phoneAuthenticationMethod
description: Adicione um novo método de autenticação de telefone.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cd3b1f64b1e7fdc43fd87e0faa37fdea6058ec29
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223247"
---
# <a name="create-phoneauthenticationmethod"></a>Criar phoneAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione um novo [método de autenticação de telefone](../resources/phoneauthenticationmethod.md). Um usuário pode ter apenas um telefone de cada tipo, capturado na **propriedade phoneType.** Isso significa, por exemplo, que a adição de um telefone a um usuário com um telefone `mobile` `mobile` pré-existing falhará. Além disso, um usuário sempre deve ter um `mobile` telefone antes de adicionar um `alternateMobile` telefone.

A adição de um número de telefone o disponibiliza para uso na MFA (autenticação multifatória) do Azure e na redefinição de senha de autoatendados (SSPR), se habilitada.

Além disso, se um usuário estiver habilitado pela política para usar a assinatura SMS e um número for adicionado, o sistema tentará registrar o número para uso `mobile` nesse sistema.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Permissões agindo em si mesmo

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

### <a name="permissions-acting-on-other-users"></a>Permissões atuando em outros usuários

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | UserAuthenticationMethod.ReadWrite.All |

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes funções [do Azure AD:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de [um objeto phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md) O JSON deve `phoneNumber` incluir e , mas não `phoneType` `smsSignInState` (que é somente leitura).

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|phoneNumber|String|O número de telefone para texto ou chamada para autenticação. Telefone números usam o formato "+ \<country code\> \<number\> x \<extension\> ", com extensão opcional. Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos. Os números são rejeitados ao criar/atualizar se não corresponderem ao formato necessário.|
|phoneType|Cadeia de Caracteres|Os valores possíveis são: `mobile` `alternateMobile` , e `office` .|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-phoneauthenticationmethod-from-authentication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-phoneauthenticationmethod-from-authentication-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "phoneType-value",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
