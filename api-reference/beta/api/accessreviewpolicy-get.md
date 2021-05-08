---
title: Obter accessReviewPolicy
description: Leia as propriedades e as relações de um objeto accessReviewPolicy.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c2acf367b269e47271e3f3629ed05ce283201c1c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240977"
---
# <a name="get-accessreviewpolicy"></a><span data-ttu-id="97ba7-103">Obter accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="97ba7-103">Get accessReviewPolicy</span></span>
<span data-ttu-id="97ba7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97ba7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97ba7-105">Leia as propriedades e as relações de um [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97ba7-105">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97ba7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="97ba7-106">Permissions</span></span>
<span data-ttu-id="97ba7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97ba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97ba7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97ba7-109">Permission type</span></span>|<span data-ttu-id="97ba7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97ba7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97ba7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97ba7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97ba7-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="97ba7-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="97ba7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97ba7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97ba7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97ba7-114">Not supported.</span></span>|
|<span data-ttu-id="97ba7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97ba7-115">Application</span></span>|<span data-ttu-id="97ba7-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="97ba7-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="97ba7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97ba7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/accessReviewPolicy
GET /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="97ba7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97ba7-118">Request headers</span></span>
|<span data-ttu-id="97ba7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="97ba7-119">Name</span></span>|<span data-ttu-id="97ba7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="97ba7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97ba7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="97ba7-121">Authorization</span></span>|<span data-ttu-id="97ba7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97ba7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97ba7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97ba7-124">Request body</span></span>
<span data-ttu-id="97ba7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97ba7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97ba7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="97ba7-126">Response</span></span>

<span data-ttu-id="97ba7-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewPolicy](../resources/accessreviewpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97ba7-127">If successful, this method returns a `200 OK` response code and an [accessReviewPolicy](../resources/accessreviewpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97ba7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="97ba7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97ba7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97ba7-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97ba7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="97ba7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/accessReviewPolicy
```
# <a name="c"></a>[<span data-ttu-id="97ba7-131">C#</span><span class="sxs-lookup"><span data-stu-id="97ba7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97ba7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97ba7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97ba7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97ba7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97ba7-134">Java</span><span class="sxs-lookup"><span data-stu-id="97ba7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="97ba7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="97ba7-135">Response</span></span>
<span data-ttu-id="97ba7-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="97ba7-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```

### <a name="request"></a><span data-ttu-id="97ba7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97ba7-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97ba7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="97ba7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
```
# <a name="c"></a>[<span data-ttu-id="97ba7-139">C#</span><span class="sxs-lookup"><span data-stu-id="97ba7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97ba7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97ba7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97ba7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97ba7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97ba7-142">Java</span><span class="sxs-lookup"><span data-stu-id="97ba7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="97ba7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="97ba7-143">Response</span></span>
<span data-ttu-id="97ba7-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="97ba7-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```
