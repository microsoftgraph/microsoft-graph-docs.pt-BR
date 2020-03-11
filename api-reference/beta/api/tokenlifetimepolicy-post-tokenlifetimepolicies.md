---
title: Criar tokenLifetimePolicy
description: Criar um novo tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0774e2fb497f94da56cd95130585cebfa86c9814
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589282"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="66d1e-103">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="66d1e-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="66d1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66d1e-105">Criar um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="66d1e-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66d1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66d1e-106">Permissions</span></span>

<span data-ttu-id="66d1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66d1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66d1e-109">Permission type</span></span>                        | <span data-ttu-id="66d1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66d1e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66d1e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66d1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="66d1e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="66d1e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="66d1e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66d1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d1e-114">Not supported.</span></span> |
| <span data-ttu-id="66d1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66d1e-115">Application</span></span>                            | <span data-ttu-id="66d1e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="66d1e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d1e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66d1e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="66d1e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66d1e-118">Request headers</span></span>

| <span data-ttu-id="66d1e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66d1e-119">Name</span></span>          | <span data-ttu-id="66d1e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d1e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="66d1e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="66d1e-121">Authorization</span></span> | <span data-ttu-id="66d1e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="66d1e-122">Bearer {token}</span></span> |
| <span data-ttu-id="66d1e-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="66d1e-123">Content-type</span></span> | <span data-ttu-id="66d1e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66d1e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="66d1e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66d1e-125">Request body</span></span>

<span data-ttu-id="66d1e-126">No corpo da solicitação, forneça uma representação JSON do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="66d1e-126">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66d1e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d1e-127">Response</span></span>

<span data-ttu-id="66d1e-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d1e-128">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66d1e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="66d1e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66d1e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66d1e-130">Request</span></span>

<span data-ttu-id="66d1e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d1e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66d1e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="66d1e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="66d1e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66d1e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66d1e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66d1e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="66d1e-135">C#</span><span class="sxs-lookup"><span data-stu-id="66d1e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66d1e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d1e-136">Response</span></span>

<span data-ttu-id="66d1e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66d1e-137">The following is an example of the response.</span></span>

> <span data-ttu-id="66d1e-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66d1e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
