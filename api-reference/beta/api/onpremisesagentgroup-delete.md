---
title: Excluir onPremisesAgentGroup
description: Excluir um objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba173597540597314ca832d0904f2ee34eb517a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977013"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="7acc6-103">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="7acc6-103">Delete onPremisesAgentGroup</span></span>

<span data-ttu-id="7acc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7acc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7acc6-105">Excluir um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="7acc6-105">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7acc6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7acc6-106">Permissions</span></span>

<span data-ttu-id="7acc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7acc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7acc6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7acc6-109">Permission type</span></span>                        | <span data-ttu-id="7acc6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7acc6-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7acc6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7acc6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7acc6-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7acc6-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="7acc6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7acc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7acc6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7acc6-114">Not supported.</span></span> |
| <span data-ttu-id="7acc6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7acc6-115">Application</span></span>                            | <span data-ttu-id="7acc6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7acc6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7acc6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7acc6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="7acc6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7acc6-118">Request headers</span></span>

| <span data-ttu-id="7acc6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7acc6-119">Name</span></span>          | <span data-ttu-id="7acc6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7acc6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7acc6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7acc6-121">Authorization</span></span> | <span data-ttu-id="7acc6-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="7acc6-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7acc6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7acc6-123">Request body</span></span>

<span data-ttu-id="7acc6-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7acc6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7acc6-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7acc6-125">Response</span></span>

<span data-ttu-id="7acc6-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7acc6-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7acc6-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7acc6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7acc6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7acc6-129">Request</span></span>

<span data-ttu-id="7acc6-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7acc6-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7acc6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7acc6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="c"></a>[<span data-ttu-id="7acc6-132">C#</span><span class="sxs-lookup"><span data-stu-id="7acc6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7acc6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7acc6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7acc6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7acc6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7acc6-135">Java</span><span class="sxs-lookup"><span data-stu-id="7acc6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7acc6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7acc6-136">Response</span></span>

<span data-ttu-id="7acc6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7acc6-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


