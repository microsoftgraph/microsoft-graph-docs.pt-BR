---
title: Criar reviewset
description: Criar um conjunto de análise de descoberta eletrônica.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 986a60dfedf05455074f386ec99caea333401711
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981242"
---
# <a name="create-reviewset"></a><span data-ttu-id="42cd6-103">Criar reviewset</span><span class="sxs-lookup"><span data-stu-id="42cd6-103">Create reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42cd6-104">Criar um novo objeto [reviewset](../resources/reviewset.md) .</span><span class="sxs-lookup"><span data-stu-id="42cd6-104">Create a new [reviewSet](../resources/reviewset.md) object.</span></span> <span data-ttu-id="42cd6-105">O corpo da solicitação contém o nome de exibição do conjunto de revisão, que é a única propriedade gravável.</span><span class="sxs-lookup"><span data-stu-id="42cd6-105">The request body contains the display name of the review set, which is the only writable property.</span></span>

## <a name="permissions"></a><span data-ttu-id="42cd6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42cd6-106">Permissions</span></span>

<span data-ttu-id="42cd6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42cd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42cd6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42cd6-109">Permission type</span></span>                        | <span data-ttu-id="42cd6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42cd6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42cd6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42cd6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42cd6-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="42cd6-112">User.Read</span></span> |
| <span data-ttu-id="42cd6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42cd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42cd6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42cd6-114">Not supported.</span></span> |
| <span data-ttu-id="42cd6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42cd6-115">Application</span></span>                            | <span data-ttu-id="42cd6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42cd6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42cd6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42cd6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42cd6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42cd6-118">Request headers</span></span>

| <span data-ttu-id="42cd6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="42cd6-119">Name</span></span>       | <span data-ttu-id="42cd6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42cd6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="42cd6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42cd6-121">Authorization</span></span> | <span data-ttu-id="42cd6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42cd6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42cd6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42cd6-124">Request body</span></span>

<span data-ttu-id="42cd6-125">No corpo da solicitação, forneça a representação JSON do [reviewset](../resources/reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="42cd6-125">In the request body, supply JSON representation of the [reviewSet](../resources/reviewset.md).</span></span>  <span data-ttu-id="42cd6-126">A tabela a seguir lista as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="42cd6-126">The following table lists the required properties.</span></span>

| <span data-ttu-id="42cd6-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42cd6-127">Property</span></span>     | <span data-ttu-id="42cd6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="42cd6-128">Type</span></span>        | <span data-ttu-id="42cd6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="42cd6-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="42cd6-130">displayName</span><span class="sxs-lookup"><span data-stu-id="42cd6-130">displayName</span></span>  | <span data-ttu-id="42cd6-131">string</span><span class="sxs-lookup"><span data-stu-id="42cd6-131">string</span></span>      | <span data-ttu-id="42cd6-132">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="42cd6-132">The name of the review set.</span></span> |

## <a name="response"></a><span data-ttu-id="42cd6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="42cd6-133">Response</span></span>

<span data-ttu-id="42cd6-134">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [reviewset](../resources/reviewset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42cd6-134">If successful, this method returns a `201 Created` response code and a [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42cd6-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42cd6-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42cd6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42cd6-136">Request</span></span>

<span data-ttu-id="42cd6-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42cd6-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42cd6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="42cd6-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewset"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
Content-type: application/json

{
  "displayName": "My Reviewset 3",
}
```
# <a name="c"></a>[<span data-ttu-id="42cd6-139">C#</span><span class="sxs-lookup"><span data-stu-id="42cd6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42cd6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42cd6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42cd6-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42cd6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42cd6-142">Java</span><span class="sxs-lookup"><span data-stu-id="42cd6-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42cd6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="42cd6-143">Response</span></span>

<span data-ttu-id="42cd6-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42cd6-144">The following is an example of the response.</span></span>

> <span data-ttu-id="42cd6-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42cd6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


