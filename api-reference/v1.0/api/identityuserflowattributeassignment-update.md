---
title: Atualizar identityUserFlowAttributeAssignment
description: Atualize as propriedades de um objeto userAttributeAssignments.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 42ca1bd9d646e99fb254ad01c0c00512fbba441e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882784"
---
# <a name="update-identityuserflowattributeassignment"></a>Atualizar identityUserFlowAttributeAssignment

Namespace: microsoft.graph

Atualize as propriedades de um objeto identityUserFlowAttributeAssignment.

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
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)

A tabela a seguir mostra as propriedades disponíveis para atualização na [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da identityUserFlowAttribute em um fluxo de usuário.|
|isOptional|Booliano|Determina se identityUserFlowAttribute é opcional. `true` significa que o usuário não precisa fornecer um valor. `false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.|
|requiresVerification|Booliano|Determina se identityUserFlowAttribute requer verificação. Isso só é usado para verificar o número de telefone ou o endereço de email do usuário.|
|userAttributeValues|[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)|As opções de entrada para o atributo de fluxo do usuário. Aplicável somente quando o userInputType `radioSingleSelect` for `dropdownSingleSelect` , ou `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|O tipo de entrada do atributo de fluxo do usuário. Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
