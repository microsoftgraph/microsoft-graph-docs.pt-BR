---
title: Atualizar ícone
description: Atualize as propriedades do objeto de ícone.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 38abc579f9195244a88ee4d56b9881f0df3c1c96
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040861"
---
# <a name="update-icon"></a><span data-ttu-id="2836a-103">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="2836a-103">Update icon</span></span>

<span data-ttu-id="2836a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2836a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2836a-105">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="2836a-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2836a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2836a-106">Permissions</span></span>
<span data-ttu-id="2836a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2836a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2836a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2836a-109">Permission type</span></span>      | <span data-ttu-id="2836a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2836a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2836a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2836a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2836a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2836a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2836a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2836a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2836a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2836a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2836a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2836a-115">Application</span></span> | <span data-ttu-id="2836a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2836a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2836a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2836a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="2836a-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2836a-118">Optional request headers</span></span>
| <span data-ttu-id="2836a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2836a-119">Name</span></span>       | <span data-ttu-id="2836a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2836a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2836a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2836a-121">Authorization</span></span>  | <span data-ttu-id="2836a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2836a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2836a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2836a-124">Request body</span></span>
<span data-ttu-id="2836a-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2836a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2836a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2836a-128">Property</span></span>     | <span data-ttu-id="2836a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2836a-129">Type</span></span>   |<span data-ttu-id="2836a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2836a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2836a-131">index</span><span class="sxs-lookup"><span data-stu-id="2836a-131">index</span></span>|<span data-ttu-id="2836a-132">int</span><span class="sxs-lookup"><span data-stu-id="2836a-132">int</span></span>|<span data-ttu-id="2836a-133">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="2836a-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="2836a-134">set</span><span class="sxs-lookup"><span data-stu-id="2836a-134">set</span></span>|<span data-ttu-id="2836a-135">string</span><span class="sxs-lookup"><span data-stu-id="2836a-135">string</span></span>|<span data-ttu-id="2836a-p104">Representa o conjunto do qual o ícone faz parte. Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles` e `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="2836a-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="2836a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2836a-138">Response</span></span>

<span data-ttu-id="2836a-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workbookIcon](../resources/workbookicon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2836a-139">If successful, this method returns a `200 OK` response code and updated [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2836a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2836a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2836a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2836a-141">Request</span></span>
<span data-ttu-id="2836a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2836a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="2836a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2836a-143">Response</span></span>
<span data-ttu-id="2836a-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2836a-144">Here is an example of the response.</span></span> <span data-ttu-id="2836a-145">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2836a-145">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


