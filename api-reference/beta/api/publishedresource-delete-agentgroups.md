---
title: Remover publishedResource de um onPremisesAgentGroup
description: Remova um [objeto publishedResource](../resources/publishedresource.md) de um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f7ac461d17ac14f97c0043381ad565614c4c09d1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132458"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="f7ecd-103">Remover publishedResource de um onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f7ecd-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

<span data-ttu-id="f7ecd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ecd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7ecd-105">Remova um [objeto publishedResource](../resources/publishedresource.md) de um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-105">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7ecd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7ecd-106">Permissions</span></span>

<span data-ttu-id="f7ecd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7ecd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7ecd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7ecd-109">Permission type</span></span>                        | <span data-ttu-id="f7ecd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="f7ecd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7ecd-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ecd-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f7ecd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7ecd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7ecd-114">Not supported.</span></span> |
| <span data-ttu-id="f7ecd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7ecd-115">Application</span></span>                            | <span data-ttu-id="f7ecd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7ecd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7ecd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7ecd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f7ecd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7ecd-118">Request headers</span></span>

| <span data-ttu-id="f7ecd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f7ecd-119">Name</span></span>          | <span data-ttu-id="f7ecd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7ecd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7ecd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7ecd-121">Authorization</span></span> | <span data-ttu-id="f7ecd-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f7ecd-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7ecd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7ecd-123">Request body</span></span>

<span data-ttu-id="f7ecd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7ecd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7ecd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7ecd-125">Response</span></span>

<span data-ttu-id="f7ecd-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7ecd-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f7ecd-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7ecd-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7ecd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7ecd-128">Request</span></span>

<span data-ttu-id="f7ecd-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7ecd-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7ecd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7ecd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="f7ecd-131">C#</span><span class="sxs-lookup"><span data-stu-id="f7ecd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7ecd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7ecd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7ecd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7ecd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7ecd-134">Java</span><span class="sxs-lookup"><span data-stu-id="f7ecd-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onpremisesagentgroup-from-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7ecd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7ecd-135">Response</span></span>

<span data-ttu-id="f7ecd-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7ecd-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



