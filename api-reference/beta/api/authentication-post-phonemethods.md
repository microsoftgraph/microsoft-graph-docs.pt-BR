---
title: Criar phoneAuthenticationMethod
description: Adicione um novo método de autenticação de telefone.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a855289f058454c0e7ff1fb301349f9e49ee12e6
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589226"
---
# <a name="create-phoneauthenticationmethod"></a>Criar phoneAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione um novo [método de autenticação de telefone](../resources/phoneauthenticationmethod.md). Um usuário pode ter apenas um telefone de cada tipo, capturado na propriedade **PhoneType** . Isso significa que, por exemplo, adicionar um `mobile` telefone a um usuário com um telefone preexistente `mobile` falhará. Além disso, um usuário deve sempre ter um `mobile` telefone antes de adicionar um `alternateMobile` telefone.

Adicionar um número de telefone o torna disponível para uso na autenticação multifator do Azure (MFA) e redefinição de senha de autoatendimento (SSPR), se habilitada.

Além disso, se um usuário estiver habilitado por política para usar a entrada do SMS e um `mobile` número for adicionado, o sistema tentará registrar o número para uso nesse sistema.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões que atuam em si (de menos para mais privilégios) | Permissões que atuam em outros (de menos para mais privilégios)|
|:---------------------------------------|:-------------------------|:-----------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. | UserAuthenticationMethod. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. | Sem suporte. |
| Aplicativo                            | Sem suporte. | Sem suporte. |

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id}/authentication/phoneMethods
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) . O JSON deve incluir `phoneNumber` e `phoneType` , mas não `smsSignInState` (que é somente leitura).

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|phoneNumber|String|O número de telefone para texto ou chamada para autenticação. Os números de telefone usam o formato "+ \<country code\> \<number\> x \<extension\> ", com a extensão opcional. Por exemplo, + 1 5555551234 ou + 1 5555551234x123 são válidas. Os números são rejeitados ao criar/atualizar se não coincidem com o formato necessário.|
|PhoneType|String|Os valores possíveis são: `mobile` , `alternateMobile` , e `office` .|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.

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

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

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
