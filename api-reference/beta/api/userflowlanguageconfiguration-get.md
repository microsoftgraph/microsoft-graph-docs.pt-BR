---
title: Obter userFlowLanguageConfiguration
description: Leia as propriedades e os relacionamentos de um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) .
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d25533822a5f67cdfc98564a41e7f53b3be98208
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706221"
---
# <a name="get-userflowlanguageconfiguration"></a>Obter userFlowLanguageConfiguration

Namespace: microsoft.graph

Leia as propriedades e os relacionamentos de um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) . Esses objetos representam um idioma disponível em um fluxo de usuário.

**Observação:** Para recuperar um idioma com suporte para personalização, você deve primeiro habilitar a personalização de idioma em seu fluxo de usuário do Azure AD B2C. Para obter mais informações, consulte [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md). A personalização de idioma é habilitada por padrão em [fluxos de usuário do Azure Active Directory](../resources/b2xidentityuserflow.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de fluxo de usuário de identidade externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_Customer')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
