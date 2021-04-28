---
title: Atualizar ícone
description: Atualize as propriedades do objeto de ícone.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 619502932eddf6e70e3b35e1532a44ed642bb891
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053990"
---
# <a name="update-icon"></a><span data-ttu-id="c76ff-103">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="c76ff-103">Update icon</span></span>

<span data-ttu-id="c76ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c76ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c76ff-105">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="c76ff-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c76ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c76ff-106">Permissions</span></span>
<span data-ttu-id="c76ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c76ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c76ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c76ff-109">Permission type</span></span>      | <span data-ttu-id="c76ff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c76ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c76ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c76ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c76ff-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c76ff-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c76ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c76ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c76ff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c76ff-114">Not supported.</span></span>    |
|<span data-ttu-id="c76ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c76ff-115">Application</span></span> | <span data-ttu-id="c76ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c76ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c76ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c76ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="c76ff-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c76ff-118">Optional request headers</span></span>
| <span data-ttu-id="c76ff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c76ff-119">Name</span></span>       | <span data-ttu-id="c76ff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76ff-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c76ff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c76ff-121">Authorization</span></span>  | <span data-ttu-id="c76ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c76ff-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c76ff-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c76ff-124">Request body</span></span>
<span data-ttu-id="c76ff-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c76ff-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c76ff-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c76ff-128">Property</span></span>     | <span data-ttu-id="c76ff-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c76ff-129">Type</span></span>   |<span data-ttu-id="c76ff-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76ff-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c76ff-131">index</span><span class="sxs-lookup"><span data-stu-id="c76ff-131">index</span></span>|<span data-ttu-id="c76ff-132">int</span><span class="sxs-lookup"><span data-stu-id="c76ff-132">int</span></span>|<span data-ttu-id="c76ff-133">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="c76ff-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="c76ff-134">set</span><span class="sxs-lookup"><span data-stu-id="c76ff-134">set</span></span>|<span data-ttu-id="c76ff-135">string</span><span class="sxs-lookup"><span data-stu-id="c76ff-135">string</span></span>|<span data-ttu-id="c76ff-136">Representa o conjunto do qual ícone faz parte.</span><span class="sxs-lookup"><span data-stu-id="c76ff-136">Represents the set that the icon is part of.</span></span> <span data-ttu-id="c76ff-137">Os valores possíveis são: `Invalid` , , , , , , , , , `ThreeArrows` , `ThreeArrowsGray` , , , , `ThreeFlags` , , `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` , `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` `FourTrafficLights` `FiveArrows` `FiveArrowsGray` `FiveRating` `FiveQuarters` , `ThreeStars` `ThreeTriangles` `FiveBoxes`</span><span class="sxs-lookup"><span data-stu-id="c76ff-137">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="c76ff-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c76ff-138">Response</span></span>

<span data-ttu-id="c76ff-139">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [Icon](../resources/icon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c76ff-139">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c76ff-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c76ff-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c76ff-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c76ff-141">Request</span></span>
<span data-ttu-id="c76ff-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c76ff-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="c76ff-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c76ff-143">Response</span></span>
<span data-ttu-id="c76ff-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c76ff-144">Here is an example of the response.</span></span> <span data-ttu-id="c76ff-145">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c76ff-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

