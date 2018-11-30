---
title: Atualizar ícone
description: Atualize as propriedades do objeto de ícone.
ms.openlocfilehash: 0cb3b1af0369c86290c842232acc57792d1552ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006974"
---
# <a name="update-icon"></a><span data-ttu-id="2692b-103">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="2692b-103">Update icon</span></span>

<span data-ttu-id="2692b-104">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="2692b-104">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2692b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2692b-105">Permissions</span></span>
<span data-ttu-id="2692b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2692b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2692b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2692b-108">Permission type</span></span>      | <span data-ttu-id="2692b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2692b-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2692b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2692b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2692b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2692b-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="2692b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2692b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2692b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2692b-113">Not supported.</span></span>    | 
|<span data-ttu-id="2692b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2692b-114">Application</span></span> | <span data-ttu-id="2692b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2692b-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2692b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2692b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="2692b-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2692b-117">Optional request headers</span></span>
| <span data-ttu-id="2692b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2692b-118">Name</span></span>       | <span data-ttu-id="2692b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2692b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2692b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2692b-120">Authorization</span></span>  | <span data-ttu-id="2692b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2692b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2692b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2692b-123">Request body</span></span>
<span data-ttu-id="2692b-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2692b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2692b-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2692b-127">Property</span></span>     | <span data-ttu-id="2692b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2692b-128">Type</span></span>   |<span data-ttu-id="2692b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2692b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2692b-130">índice</span><span class="sxs-lookup"><span data-stu-id="2692b-130">index</span></span>|<span data-ttu-id="2692b-131">inteiro</span><span class="sxs-lookup"><span data-stu-id="2692b-131">int</span></span>|<span data-ttu-id="2692b-132">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="2692b-132">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="2692b-133">set</span><span class="sxs-lookup"><span data-stu-id="2692b-133">set</span></span>|<span data-ttu-id="2692b-134">string</span><span class="sxs-lookup"><span data-stu-id="2692b-134">string</span></span>|<span data-ttu-id="2692b-135">Representa o que o ícone faz parte do conjunto.</span><span class="sxs-lookup"><span data-stu-id="2692b-135">Represents the set that the icon is part of.</span></span> <span data-ttu-id="2692b-136">Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars` , `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="2692b-136">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="2692b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2692b-137">Response</span></span>

<span data-ttu-id="2692b-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Icon](../resources/icon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2692b-138">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2692b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2692b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2692b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2692b-140">Request</span></span>
<span data-ttu-id="2692b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2692b-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2692b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2692b-142">Response</span></span>
<span data-ttu-id="2692b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2692b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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