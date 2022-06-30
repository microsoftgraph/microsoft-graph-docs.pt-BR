---
title: Excluir internalDomainFederation
description: Exclua um objeto internalDomainFederation.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 631984680cb7b84320681d317888e39c92ac5118
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447403"
---
# <a name="delete-internaldomainfederation"></a>Excluir internalDomainFederation
Namespace: microsoft.graph

[Exclua um objeto internalDomainFederation](../resources/internaldomainfederation.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Domain.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /domains/{domainsId}/federationConfiguration/{internalDomainFederationId}
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
  "name": "delete_internaldomainfederation"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com/federationConfiguration/96db02e2-80c1-5555-bc3a-de92ffb8c5be
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

