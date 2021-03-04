---
title: Criar activityBasedTimeoutPolicy
description: Crie uma nova activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 40ca870f0ca8f65578723a2bc613077d735700e7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438978"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="27bf5-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="27bf5-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="27bf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27bf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27bf5-105">Crie um novo [objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27bf5-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27bf5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="27bf5-106">Permissions</span></span>

<span data-ttu-id="27bf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27bf5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27bf5-109">Permission type</span></span>                        | <span data-ttu-id="27bf5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27bf5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27bf5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27bf5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27bf5-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="27bf5-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="27bf5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27bf5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27bf5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27bf5-114">Not supported.</span></span> |
| <span data-ttu-id="27bf5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27bf5-115">Application</span></span>                            | <span data-ttu-id="27bf5-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="27bf5-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="27bf5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27bf5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="27bf5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27bf5-118">Request headers</span></span>

| <span data-ttu-id="27bf5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="27bf5-119">Name</span></span>          | <span data-ttu-id="27bf5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27bf5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27bf5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="27bf5-121">Authorization</span></span> | <span data-ttu-id="27bf5-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="27bf5-122">Bearer {token}</span></span> |
| <span data-ttu-id="27bf5-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="27bf5-123">Content-type</span></span> | <span data-ttu-id="27bf5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27bf5-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="27bf5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27bf5-125">Request body</span></span>

<span data-ttu-id="27bf5-126">No corpo da solicitação, fornece uma representação JSON do [objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="27bf5-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27bf5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="27bf5-127">Response</span></span>

<span data-ttu-id="27bf5-128">Se tiver êxito, este método retornará um código de `201 Created` resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27bf5-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27bf5-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27bf5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27bf5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27bf5-130">Request</span></span>

<span data-ttu-id="27bf5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27bf5-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27bf5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="27bf5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="27bf5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27bf5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27bf5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27bf5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="27bf5-135">C#</span><span class="sxs-lookup"><span data-stu-id="27bf5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27bf5-136">Java</span><span class="sxs-lookup"><span data-stu-id="27bf5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27bf5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="27bf5-137">Response</span></span>

<span data-ttu-id="27bf5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27bf5-138">The following is an example of the response.</span></span>

> <span data-ttu-id="27bf5-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27bf5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


