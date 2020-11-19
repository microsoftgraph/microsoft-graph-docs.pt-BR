---
title: Criar emailAuthenticationMethod
description: Criar um novo objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e66a0254240c852ab364a97d5d246f2714687afe
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352151"
---
# <a name="create-emailauthenticationmethod"></a>Criar emailAuthenticationMethod
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Definir o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) de um usuário. A autenticação de email é um método de redefinição de senha de autoatendimento. Um usuário pode ter apenas um método de autenticação de email.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões que atuam em si (de a mais de privilégios mínimos)|Permissões que atuam em outros (de menos para mais privilégios)|
|:---|:---|:--|
|Delegado (conta corporativa ou de estudante)|Sem suporte.|UserAuthenticationMethod. ReadWrite. All
|Delegado (conta pessoal da Microsoft)|Sem suporte.|Sem suporte.
|Aplicativo|Sem suporte.|Sem suporte.

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) com o endereço de email desejado.

A tabela a seguir mostra as propriedades que são necessárias ao criar [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|emailAddress|String|Endereço de email|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
