---
title: Atualizar publishedResource
description: Atualiza as propriedades de um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e0492116ad0d012846fe1ac531ddcbf4bb77b95
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840979"
---
# <a name="update-publishedresource"></a><span data-ttu-id="393bd-103">Atualizar publishedResource</span><span class="sxs-lookup"><span data-stu-id="393bd-103">Update publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393bd-104">Atualize as propriedades do objeto publishedresource [publishedresource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="393bd-104">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="393bd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="393bd-105">Permissions</span></span>

<span data-ttu-id="393bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="393bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="393bd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="393bd-108">Permission type</span></span>                        | <span data-ttu-id="393bd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="393bd-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="393bd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="393bd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="393bd-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="393bd-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="393bd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="393bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="393bd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="393bd-113">Not supported.</span></span> |
| <span data-ttu-id="393bd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="393bd-114">Application</span></span>                            | <span data-ttu-id="393bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="393bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="393bd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="393bd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="393bd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="393bd-117">Request headers</span></span>

| <span data-ttu-id="393bd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="393bd-118">Name</span></span>       | <span data-ttu-id="393bd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="393bd-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="393bd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="393bd-120">Authorization</span></span> | <span data-ttu-id="393bd-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="393bd-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="393bd-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="393bd-122">Request body</span></span>

<span data-ttu-id="393bd-123">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="393bd-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="393bd-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="393bd-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="393bd-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="393bd-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="393bd-126">A tabela a seguir lista as propriedades que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="393bd-126">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="393bd-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="393bd-127">Property</span></span>     | <span data-ttu-id="393bd-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="393bd-128">Type</span></span>        | <span data-ttu-id="393bd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="393bd-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="393bd-130">displayName</span><span class="sxs-lookup"><span data-stu-id="393bd-130">displayName</span></span>|<span data-ttu-id="393bd-131">String</span><span class="sxs-lookup"><span data-stu-id="393bd-131">String</span></span>|<span data-ttu-id="393bd-132">Representa um nome de recurso publicado no local.</span><span class="sxs-lookup"><span data-stu-id="393bd-132">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="393bd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="393bd-133">Response</span></span>

<span data-ttu-id="393bd-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="393bd-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="393bd-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="393bd-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="393bd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="393bd-136">Request</span></span>

<span data-ttu-id="393bd-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="393bd-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="393bd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="393bd-138">Response</span></span>

<span data-ttu-id="393bd-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="393bd-139">The following is an example of the response.</span></span>

> <span data-ttu-id="393bd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="393bd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
