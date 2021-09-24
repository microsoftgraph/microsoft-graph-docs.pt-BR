---
title: Excluir cloudPcProvisioningPolicy
description: Exclua um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3115719fc57ba4682133a56e4076762742af38a5
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508261"
---
# <a name="delete-cloudpcprovisioningpolicy"></a>Excluir cloudPcProvisioningPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Exclua um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md) Você não poderá excluir uma política que estiver em uso.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
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


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-provisioningpolicies-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-provisioningpolicies-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-provisioningpolicies-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-provisioningpolicies-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
