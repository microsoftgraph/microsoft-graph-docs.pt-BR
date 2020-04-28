---
title: Criar activityBasedTimeoutPolicy
description: Criar um novo activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d6c8bcecd10d91c4298635d9268e0b3fe7688633
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916342"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="cf19a-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="cf19a-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="cf19a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf19a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf19a-105">Criar um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cf19a-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf19a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf19a-106">Permissions</span></span>

<span data-ttu-id="cf19a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf19a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf19a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf19a-109">Permission type</span></span>                        | <span data-ttu-id="cf19a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf19a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf19a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf19a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf19a-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf19a-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="cf19a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf19a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf19a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf19a-114">Not supported.</span></span> |
| <span data-ttu-id="cf19a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf19a-115">Application</span></span>                            | <span data-ttu-id="cf19a-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf19a-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf19a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf19a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cf19a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf19a-118">Request headers</span></span>

| <span data-ttu-id="cf19a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cf19a-119">Name</span></span>          | <span data-ttu-id="cf19a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf19a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cf19a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf19a-121">Authorization</span></span> | <span data-ttu-id="cf19a-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="cf19a-122">Bearer {token}</span></span> |
| <span data-ttu-id="cf19a-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="cf19a-123">Content-type</span></span> | <span data-ttu-id="cf19a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf19a-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf19a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf19a-125">Request body</span></span>

<span data-ttu-id="cf19a-126">No corpo da solicitação, forneça uma representação JSON do objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cf19a-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cf19a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf19a-127">Response</span></span>

<span data-ttu-id="cf19a-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf19a-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf19a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cf19a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf19a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf19a-130">Request</span></span>

<span data-ttu-id="cf19a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf19a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf19a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf19a-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="cf19a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf19a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf19a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf19a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cf19a-135">C#</span><span class="sxs-lookup"><span data-stu-id="cf19a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf19a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf19a-136">Response</span></span>

<span data-ttu-id="cf19a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf19a-137">The following is an example of the response.</span></span>

> <span data-ttu-id="cf19a-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf19a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
