---
title: Criar idiomas
description: Crie um idioma personalizado em um fluxo de usuário do Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1edc89a4de37805bc150e2d0fc9f0a2c74b262da
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843900"
---
# <a name="create-languages"></a>Criar idiomas

Namespace: microsoft.graph

Esse método é usado para criar ou atualizar um idioma personalizado em um fluxo de usuário do Azure AD B2C.

**Observação:** Você deve habilitar a personalização de idioma no fluxo de usuários do Azure AD B2C antes de criar um idioma personalizado. Para obter mais informações, [consulte Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de Fluxo de Usuário de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)

A tabela a seguir mostra as propriedades que podem ser fornecidas opcionalmente ao criar [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do idioma. Esse campo é compatível com a marca de identificação de idioma [RFC 5646](https://tools.ietf.org/html/rfc5646) e deve ser uma ID de idioma documentada. Se fornecido no corpo da solicitação, ele deve corresponder ao identificador fornecido na URL da solicitação.|
|isEnabled|Booliano|Indica se o idioma está habilitado dentro do fluxo do usuário. Se isso não for fornecido na solicitação, isEnabled será definido como "true".|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a>Exemplo 1: Criar um idioma personalizado em um fluxo de usuário do Azure AD B2C

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "id": "es-ES",
  "isEnabled": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages/$entity",
  "id": "es-ES",
  "isEnabled": true,
  "displayName": "Spanish (Spain)"
}
```

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a>Exemplo 2: Atualizar um idioma personalizado em um fluxo de usuário do Azure AD B2C

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "isEnabled": false
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
