---
title: Atualizar publishedResource
description: Atualiza as propriedades de um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2645e33b4b5a91607ab1f682c8b70e7485163fb4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412324"
---
# <a name="update-publishedresource"></a><span data-ttu-id="adf3e-103">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="adf3e-103">Update publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adf3e-104">Atualize as propriedades do objeto publishedresource [publishedresource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="adf3e-104">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="adf3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="adf3e-105">Permissions</span></span>

<span data-ttu-id="adf3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adf3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adf3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adf3e-108">Permission type</span></span>                        | <span data-ttu-id="adf3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adf3e-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="adf3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adf3e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="adf3e-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="adf3e-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="adf3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adf3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adf3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adf3e-113">Not supported.</span></span> |
| <span data-ttu-id="adf3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adf3e-114">Application</span></span>                            | <span data-ttu-id="adf3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adf3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="adf3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adf3e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="adf3e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adf3e-117">Request headers</span></span>

| <span data-ttu-id="adf3e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="adf3e-118">Name</span></span>       | <span data-ttu-id="adf3e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="adf3e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="adf3e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="adf3e-120">Authorization</span></span> | <span data-ttu-id="adf3e-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="adf3e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="adf3e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adf3e-122">Request body</span></span>

<span data-ttu-id="adf3e-123">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="adf3e-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="adf3e-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="adf3e-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="adf3e-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="adf3e-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="adf3e-126">A tabela a seguir lista as propriedades que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="adf3e-126">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="adf3e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adf3e-127">Property</span></span>     | <span data-ttu-id="adf3e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="adf3e-128">Type</span></span>        | <span data-ttu-id="adf3e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="adf3e-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="adf3e-130">displayName</span><span class="sxs-lookup"><span data-stu-id="adf3e-130">displayName</span></span>|<span data-ttu-id="adf3e-131">String</span><span class="sxs-lookup"><span data-stu-id="adf3e-131">String</span></span>|<span data-ttu-id="adf3e-132">Representa um nome de recurso publicado no local.</span><span class="sxs-lookup"><span data-stu-id="adf3e-132">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="adf3e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="adf3e-133">Response</span></span>

<span data-ttu-id="adf3e-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="adf3e-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="adf3e-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="adf3e-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adf3e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adf3e-136">Request</span></span>

<span data-ttu-id="adf3e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="adf3e-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="adf3e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="adf3e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_publishedresource"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d

{
    "displayName": "Demo provisioning (updated)"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adf3e-139">C#</span><span class="sxs-lookup"><span data-stu-id="adf3e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adf3e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adf3e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adf3e-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="adf3e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="adf3e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="adf3e-142">Response</span></span>

<span data-ttu-id="adf3e-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="adf3e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="adf3e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adf3e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update publishedresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
