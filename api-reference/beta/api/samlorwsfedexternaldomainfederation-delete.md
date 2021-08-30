---
title: Excluir samlOrWsFedExternalDomainFederation
description: Exclua um objeto samlOrWsFedExternalDomainFederation.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 98365e11649c5e4bd90ad2893a53a9c65fa36fc1
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697002"
---
# <a name="delete-samlorwsfedexternaldomainfederation"></a>Excluir samlOrWsFedExternalDomainFederation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Exclua um objeto samlOrWsFedExternalDomainFederation.](../resources/samlorwsfedexternaldomainfederation.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|Domain.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes [funções Azure Active Directory (Azure AD)](/azure/active-directory/roles/permissions-reference):

* Administrador global
* Administrador do Provedor de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE directory/federationConfigurations/{samlOrWsFedExternalDomainFederation ID}
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
  "name": "delete_samlorwsfedexternaldomainfederation"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/directory/federationConfigurations/96db02e2-80c1-5555-bc3a-de92ffb8c5be
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
