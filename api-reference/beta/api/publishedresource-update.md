---
title: Atualizar publishedResource
description: Atualiza as propriedades de um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f73a78c3d22e900a4c114dc07edded66bfc91318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454819"
---
# <a name="update-publishedresource"></a><span data-ttu-id="d5939-103">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="d5939-103">Update publishedResource</span></span>

<span data-ttu-id="d5939-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d5939-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5939-105">Atualize as propriedades do objeto publishedresource [publishedresource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="d5939-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5939-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5939-106">Permissions</span></span>

<span data-ttu-id="d5939-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5939-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5939-109">Permission type</span></span>                        | <span data-ttu-id="d5939-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5939-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="d5939-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5939-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5939-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5939-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="d5939-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5939-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5939-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5939-114">Not supported.</span></span> |
| <span data-ttu-id="d5939-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5939-115">Application</span></span>                            | <span data-ttu-id="d5939-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5939-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5939-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5939-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="d5939-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5939-118">Request headers</span></span>

| <span data-ttu-id="d5939-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5939-119">Name</span></span>       | <span data-ttu-id="d5939-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5939-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d5939-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5939-121">Authorization</span></span> | <span data-ttu-id="d5939-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d5939-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5939-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5939-123">Request body</span></span>

<span data-ttu-id="d5939-124">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="d5939-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="d5939-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d5939-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d5939-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d5939-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="d5939-127">A tabela a seguir lista as propriedades que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d5939-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="d5939-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5939-128">Property</span></span>     | <span data-ttu-id="d5939-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5939-129">Type</span></span>        | <span data-ttu-id="d5939-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5939-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d5939-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d5939-131">displayName</span></span>|<span data-ttu-id="d5939-132">String</span><span class="sxs-lookup"><span data-stu-id="d5939-132">String</span></span>|<span data-ttu-id="d5939-133">Representa um nome de recurso publicado no local.</span><span class="sxs-lookup"><span data-stu-id="d5939-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="d5939-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5939-134">Response</span></span>

<span data-ttu-id="d5939-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5939-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d5939-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d5939-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5939-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5939-137">Request</span></span>

<span data-ttu-id="d5939-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5939-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5939-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5939-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d5939-140">C#</span><span class="sxs-lookup"><span data-stu-id="d5939-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5939-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5939-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5939-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5939-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5939-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5939-143">Response</span></span>

<span data-ttu-id="d5939-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5939-144">The following is an example of the response.</span></span>

> <span data-ttu-id="d5939-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5939-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
