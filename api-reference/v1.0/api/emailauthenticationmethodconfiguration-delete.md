---
title: Excluir emailAuthenticationMethodConfiguration
description: Exclui um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b25e0545eba722ab251a450600eb587d2ebad35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964575"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a>Excluir emailAuthenticationMethodConfiguration

Namespace: microsoft.graph

Remova as alterações feitas na política de método [de autenticação de email](../resources/emailauthenticationmethodconfiguration.md) revertendo a política para sua configuração padrão.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Policy.ReadWrite.AuthenticationMethod|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.ReadWrite.AuthenticationMethod|

Para cenários delegados, o administrador precisa da função de administrador global. Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

