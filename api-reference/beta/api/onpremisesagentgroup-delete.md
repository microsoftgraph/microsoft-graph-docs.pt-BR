---
title: Excluir onPremisesAgentGroup
description: '**Exclua um objeto onPremisesAgentGroup.**'
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 97a778347065783a887de1fd9877af35081e44b8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136422"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="67eec-103">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="67eec-103">Delete onPremisesAgentGroup</span></span>

<span data-ttu-id="67eec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67eec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67eec-105">[Exclua um objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="67eec-105">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67eec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67eec-106">Permissions</span></span>

<span data-ttu-id="67eec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67eec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67eec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67eec-109">Permission type</span></span>                        | <span data-ttu-id="67eec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67eec-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="67eec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67eec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="67eec-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67eec-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="67eec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67eec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67eec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67eec-114">Not supported.</span></span> |
| <span data-ttu-id="67eec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67eec-115">Application</span></span>                            | <span data-ttu-id="67eec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67eec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67eec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67eec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="67eec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67eec-118">Request headers</span></span>

| <span data-ttu-id="67eec-119">Nome</span><span class="sxs-lookup"><span data-stu-id="67eec-119">Name</span></span>          | <span data-ttu-id="67eec-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="67eec-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="67eec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="67eec-121">Authorization</span></span> | <span data-ttu-id="67eec-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="67eec-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="67eec-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67eec-123">Request body</span></span>

<span data-ttu-id="67eec-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67eec-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67eec-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="67eec-125">Response</span></span>

<span data-ttu-id="67eec-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67eec-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67eec-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="67eec-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67eec-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67eec-129">Request</span></span>

<span data-ttu-id="67eec-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67eec-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67eec-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="67eec-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="c"></a>[<span data-ttu-id="67eec-132">C#</span><span class="sxs-lookup"><span data-stu-id="67eec-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67eec-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67eec-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67eec-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67eec-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67eec-135">Java</span><span class="sxs-lookup"><span data-stu-id="67eec-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="67eec-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="67eec-136">Response</span></span>

<span data-ttu-id="67eec-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67eec-137">The following is an example of the response.</span></span>

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



