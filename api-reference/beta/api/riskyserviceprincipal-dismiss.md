---
title: 'riskyServicePrincipal: dismiss'
description: Descartar o risco de um ou mais objetos riskyServicePrincipal.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6bdb0100d017fbb53d796520dfab5b4766da7afc
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519926"
---
# <a name="riskyserviceprincipal-dismiss"></a>riskyServicePrincipal: dismiss
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descartar o risco de um ou mais [objetos riskyServicePrincipal](../resources/riskyserviceprincipal.md) . Essa ação define o nível de risco da conta principal do serviço direcionado como `none`. Você pode descartar até 60 contas de entidade de serviço em uma solicitação.

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
POST /identityProtection/riskyServicePrincipals/dismiss
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
  "name": "riskyserviceprincipal_dismiss"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityProtection/riskyServicePrincipals/dismiss
Content-Type: application/json

{
  "servicePrincipalIds": [
    "9089a539-a539-9089-39a5-899039a58990"
  ]
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

