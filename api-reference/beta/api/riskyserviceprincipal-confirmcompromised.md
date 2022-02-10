---
title: 'riskyServicePrincipal: confirmCompromised'
description: Confirme um ou mais objetos riskyServicePrincipal como comprometidos.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c145e72603bd6a8a3da2514d0ea264905af4daac
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519929"
---
# <a name="riskyserviceprincipal-confirmcompromised"></a>riskyServicePrincipal: confirmCompromised
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Confirme um ou mais [objetos riskyServicePrincipal](../resources/riskyserviceprincipal.md) como comprometidos. Essa ação define o nível de risco da conta principal do serviço direcionado como `high`. Quando o nível de risco da entidade de serviço é confirmado como comprometido, o objeto principal do serviço é desabilitado e sua propriedade **disabledByMicrosoftStatus** é atualizada.

>**Observação:** Usar a API riskyServicePrincipal requer uma Azure AD Premium P2 de usuário.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|IdentityRiskyServicePrincipal.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyServicePrincipals/confirmCompromised
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, especifique a coleção de ids das entidades de serviço de risco em **uma propriedade servicePrincipalIds** . 

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "riskyserviceprincipal_confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityProtection/riskyServicePrincipals/confirmCompromised
Content-Type: application/json

{
  "servicePrincipalIds": [
    "9089a539-a539-9089-39a5-899039a58990"
  ]
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

