---
title: Criar identityUserFlowAttribute
description: Criar um novo objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 443ac0848e7ace309172dc0ca38d9a191acb9635
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742345"
---
# <a name="create-identityuserflowattribute"></a>Criar identityUserFlowAttribute

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow. ReadWrite. All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow. ReadWrite. All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador do atributo de fluxo do usuário de identidade externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|String|O identificador do atributo de fluxo do usuário. Este é um atributo somente leitura que é criado automaticamente.|
|displayName|String|O nome de exibição do atributo de fluxo do usuário.|
|description|String|A descrição do atributo de fluxo do usuário. Ele é mostrado ao usuário no momento da inscrição.|
|userFlowAttributeType|String|O tipo do atributo de fluxo do usuário. Este é um atributo somente leitura que é definido automaticamente. Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom` .|
|dataType|Cadeia de caracteres|O tipo de dados do atributo de fluxo do usuário. Isso não pode ser modificado depois que o atributo de fluxo do usuário personalizado é criado. Os valores com suporte para **DataType** são:<br/><ul><li>`string` : indica que o tipo de dados de identityUserFlowAttribute é uma cadeia de caracteres. </li><li>`boolean` : indica que o tipo de dados de identityUserFlowAttribute é um Boolean.</li><li>`int64` : indica que o tipo de dados de identityUserFlowAttribute é um inteiro.</li></ul>|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `201 Created` código de resposta e um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
