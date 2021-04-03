---
title: Criar featureRolloutPolicy
description: Crie um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b731778c096470f23799540919ff93f9a8e52853
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508334"
---
# <a name="create-featurerolloutpolicy"></a>Criar featureRolloutPolicy

Namespace: microsoft.graph

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Directory.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token}. Obrigatório |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [um featureRolloutPolicy](../resources/featurerolloutpolicy.md).

| Parâmetro | Tipo | Descrição|
|:---------------|:--------|:----------|
|displayName |string |O nome de exibição dessa política de lançamento de recursos.|
|feature |stagedFeatureName |O recurso que seria lançado usando essa política.|
|isEnabled |string |Indica se a adoção de recursos está habilitada.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_policies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


