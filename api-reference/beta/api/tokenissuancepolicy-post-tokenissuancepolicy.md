---
title: Criar tokenIssuancePolicy
description: Criar um novo tokenIssuancePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e02230ff52f7e9969d653f65f885de6b782c3f46
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591625"
---
# <a name="create-tokenissuancepolicy"></a><span data-ttu-id="13387-103">Criar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="13387-103">Create tokenIssuancePolicy</span></span>

<span data-ttu-id="13387-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13387-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13387-105">Criar um novo objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="13387-105">Create a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13387-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13387-106">Permissions</span></span>

<span data-ttu-id="13387-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13387-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13387-109">Permission type</span></span>                        | <span data-ttu-id="13387-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13387-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="13387-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13387-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13387-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="13387-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="13387-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13387-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13387-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13387-114">Not supported.</span></span> |
| <span data-ttu-id="13387-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13387-115">Application</span></span>                            | <span data-ttu-id="13387-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="13387-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="13387-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13387-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="13387-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13387-118">Request headers</span></span>

| <span data-ttu-id="13387-119">Nome</span><span class="sxs-lookup"><span data-stu-id="13387-119">Name</span></span>          | <span data-ttu-id="13387-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="13387-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="13387-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13387-121">Authorization</span></span> | <span data-ttu-id="13387-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13387-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13387-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="13387-124">Content-type</span></span> | <span data-ttu-id="13387-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13387-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13387-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13387-127">Request body</span></span>

<span data-ttu-id="13387-128">No corpo da solicitação, forneça uma representação JSON de um objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="13387-128">In the request body, supply a JSON representation of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="13387-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="13387-129">Response</span></span>

<span data-ttu-id="13387-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13387-130">If successful, this method returns a `201 Created` response code and a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13387-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13387-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13387-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13387-132">Request</span></span>

<span data-ttu-id="13387-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13387-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13387-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="13387-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenIssuancePolicies_from_tokenIssuancePolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="13387-135">C#</span><span class="sxs-lookup"><span data-stu-id="13387-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicies-from-tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13387-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13387-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicies-from-tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13387-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13387-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicies-from-tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="13387-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="13387-138">Response</span></span>

<span data-ttu-id="13387-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13387-139">The following is an example of the response.</span></span>

> <span data-ttu-id="13387-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13387-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
