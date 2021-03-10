---
title: Atualizar ícone
description: Atualize as propriedades do objeto de ícone.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b1a5d7d6effe0539b348b0410edc332c284490f2
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576740"
---
# <a name="update-icon"></a><span data-ttu-id="34df4-103">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="34df4-103">Update icon</span></span>

<span data-ttu-id="34df4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34df4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34df4-105">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="34df4-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34df4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34df4-106">Permissions</span></span>
<span data-ttu-id="34df4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34df4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34df4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34df4-109">Permission type</span></span>      | <span data-ttu-id="34df4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34df4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34df4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34df4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34df4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34df4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34df4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34df4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34df4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34df4-114">Not supported.</span></span>    |
|<span data-ttu-id="34df4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34df4-115">Application</span></span> | <span data-ttu-id="34df4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34df4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34df4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34df4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="34df4-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="34df4-118">Optional request headers</span></span>
| <span data-ttu-id="34df4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="34df4-119">Name</span></span>       | <span data-ttu-id="34df4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="34df4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="34df4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34df4-121">Authorization</span></span>  | <span data-ttu-id="34df4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34df4-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="34df4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34df4-124">Request body</span></span>
<span data-ttu-id="34df4-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="34df4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="34df4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34df4-128">Property</span></span>     | <span data-ttu-id="34df4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="34df4-129">Type</span></span>   |<span data-ttu-id="34df4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="34df4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34df4-131">index</span><span class="sxs-lookup"><span data-stu-id="34df4-131">index</span></span>|<span data-ttu-id="34df4-132">int</span><span class="sxs-lookup"><span data-stu-id="34df4-132">int</span></span>|<span data-ttu-id="34df4-133">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="34df4-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="34df4-134">set</span><span class="sxs-lookup"><span data-stu-id="34df4-134">set</span></span>|<span data-ttu-id="34df4-135">string</span><span class="sxs-lookup"><span data-stu-id="34df4-135">string</span></span>|<span data-ttu-id="34df4-136">Representa o conjunto do qual ícone faz parte.</span><span class="sxs-lookup"><span data-stu-id="34df4-136">Represents the set that the icon is part of.</span></span> <span data-ttu-id="34df4-137">Os valores possíveis são: `Invalid` , , , , , , , , , `ThreeArrows` , `ThreeArrowsGray` , , , , `ThreeFlags` , , `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` , `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` `FourTrafficLights` `FiveArrows` `FiveArrowsGray` `FiveRating` `FiveQuarters` , `ThreeStars` `ThreeTriangles` `FiveBoxes`</span><span class="sxs-lookup"><span data-stu-id="34df4-137">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="34df4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="34df4-138">Response</span></span>

<span data-ttu-id="34df4-139">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [Icon](../resources/icon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34df4-139">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34df4-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34df4-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34df4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34df4-141">Request</span></span>
<span data-ttu-id="34df4-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34df4-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="34df4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="34df4-143">Response</span></span>
<span data-ttu-id="34df4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34df4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

