---
title: Criar userAttributeAssignments
description: Crie um novo objeto identityUserFlowAttributeAssignment em um b2xIdentityUserFlow.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3daabfb9f384799872cf5155b97f7fc61a772b11
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990762"
---
# <a name="create-userattributeassignments"></a>Criar userAttributeAssignments

Namespace: microsoft.graph

Crie um novo objeto identityUserFlowAttributeAssignment em [um b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|IdentityUserFlow.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da identityUserFlowAttribute em um fluxo de usuário.|
|isOptional|Booliano|Determina se identityUserFlowAttribute é opcional. `true` significa que o usuário não precisa fornecer um valor. `false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.|
|requiresVerification|Booliano|Determina se identityUserFlowAttribute requer verificação. Isso só é usado para verificar o número de telefone ou o endereço de email do usuário.|
|userAttributeValues|[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)|As opções de entrada para o atributo de fluxo do usuário. Aplicável somente quando o userInputType `radioSingleSelect` for `dropdownSingleSelect` , ou `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|O tipo de entrada do atributo de fluxo do usuário. Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|O identificador do atributo de fluxo do usuário a ser incluído na atribuição de fluxo do usuário.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflowattributeassignment-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflowattributeassignment-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflowattributeassignment-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflowattributeassignment-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-identityuserflowattributeassignment-from--2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
