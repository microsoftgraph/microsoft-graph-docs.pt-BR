---
title: Atualizar fido2AuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 93ea4ad235ba58df44c33be8c64beaa294557628
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435988"
---
# <a name="update-fido2authenticationmethodconfiguration"></a>Atualizar fido2AuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um objeto [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) que representa a política de método de autenticação de Chaves de Segurança FIDO2 para o locatário do Azure AD.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

* Administrador global


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) com os valores de campos que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

Para ver a lista de propriedades que podem ser atualizadas, consulte [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).

>**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.fido2AuthenticationMethodConfiguration` corpo.


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_fido2authenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "state": "enabled",
    "isAttestationEnforced": "true"
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

