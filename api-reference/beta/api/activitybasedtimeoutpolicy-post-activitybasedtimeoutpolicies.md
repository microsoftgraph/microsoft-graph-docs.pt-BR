---
title: Criar activityBasedTimeoutPolicy
description: Criar um novo activityBasedTimeoutPolicy.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a862e485be19f432ee3a2abc8519639444e9f169
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217936"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="8169c-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="8169c-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="8169c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8169c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8169c-105">Criar um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8169c-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8169c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8169c-106">Permissions</span></span>

<span data-ttu-id="8169c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8169c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8169c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8169c-109">Permission type</span></span>                        | <span data-ttu-id="8169c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8169c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8169c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8169c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8169c-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8169c-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8169c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8169c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8169c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8169c-114">Not supported.</span></span> |
| <span data-ttu-id="8169c-115">Application</span><span class="sxs-lookup"><span data-stu-id="8169c-115">Application</span></span>                            | <span data-ttu-id="8169c-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8169c-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8169c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8169c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8169c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8169c-118">Request headers</span></span>

| <span data-ttu-id="8169c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8169c-119">Name</span></span>          | <span data-ttu-id="8169c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8169c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8169c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8169c-121">Authorization</span></span> | <span data-ttu-id="8169c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8169c-122">Bearer {token}</span></span> |
| <span data-ttu-id="8169c-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8169c-123">Content-type</span></span> | <span data-ttu-id="8169c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8169c-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8169c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8169c-125">Request body</span></span>

<span data-ttu-id="8169c-126">No corpo da solicitação, forneça uma representação JSON do objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8169c-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8169c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8169c-127">Response</span></span>

<span data-ttu-id="8169c-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8169c-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8169c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8169c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8169c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8169c-130">Request</span></span>

<span data-ttu-id="8169c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8169c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8169c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8169c-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="8169c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8169c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8169c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8169c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8169c-135">C#</span><span class="sxs-lookup"><span data-stu-id="8169c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8169c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8169c-136">Response</span></span>

<span data-ttu-id="8169c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8169c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8169c-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8169c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
