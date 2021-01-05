---
title: Atualizar b2cIdentityUserFlow
description: Atualiza as propriedades de um objeto b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fb11cd2f9dc547499091876e1bdf6130819d270
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753121"
---
# <a name="update-b2cidentityuserflow"></a>Atualizar b2cIdentityUserFlow

Namespace: microsoft.graph

Atualiza as propriedades de um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow.ReadWrite.All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de fluxo de usuário de identidade externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .

A tabela a seguir mostra as propriedades que podem ser atualizadas após a criação de um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isLanguageCustomizationEnabled|Booliano|A propriedade que determina se a personalização de idioma é habilitada dentro do fluxo do usuário do B2C. A personalização de idioma não é habilitada por padrão para os fluxos de usuário do B2C.|
|defaultLanguageTag|Cadeia de caracteres|Indica o idioma padrão do b2cIdentityUserFlow que será usado quando nenhuma `ui_locale` marca for especificada na solicitação. Esse campo é [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json
Content-length: 469

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en",
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
