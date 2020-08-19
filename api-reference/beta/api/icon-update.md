---
title: Atualizar ícone
description: Atualize as propriedades do objeto de ícone.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 9754d9223f8862e40b46b065d075eb77dd7f5c2d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807280"
---
# <a name="update-icon"></a><span data-ttu-id="26ce5-103">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="26ce5-103">Update icon</span></span>

<span data-ttu-id="26ce5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ce5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26ce5-105">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="26ce5-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="26ce5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26ce5-106">Permissions</span></span>
<span data-ttu-id="26ce5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26ce5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ce5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26ce5-109">Permission type</span></span>      | <span data-ttu-id="26ce5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26ce5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26ce5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26ce5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26ce5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26ce5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26ce5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26ce5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26ce5-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26ce5-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26ce5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26ce5-115">Application</span></span> | <span data-ttu-id="26ce5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26ce5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26ce5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26ce5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="26ce5-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="26ce5-118">Optional request headers</span></span>
| <span data-ttu-id="26ce5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26ce5-119">Name</span></span>       | <span data-ttu-id="26ce5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ce5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26ce5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26ce5-121">Authorization</span></span>  | <span data-ttu-id="26ce5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26ce5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26ce5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26ce5-124">Request body</span></span>
<span data-ttu-id="26ce5-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="26ce5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26ce5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26ce5-128">Property</span></span>     | <span data-ttu-id="26ce5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="26ce5-129">Type</span></span>   |<span data-ttu-id="26ce5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ce5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26ce5-131">index</span><span class="sxs-lookup"><span data-stu-id="26ce5-131">index</span></span>|<span data-ttu-id="26ce5-132">int</span><span class="sxs-lookup"><span data-stu-id="26ce5-132">int</span></span>|<span data-ttu-id="26ce5-133">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="26ce5-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="26ce5-134">set</span><span class="sxs-lookup"><span data-stu-id="26ce5-134">set</span></span>|<span data-ttu-id="26ce5-135">string</span><span class="sxs-lookup"><span data-stu-id="26ce5-135">string</span></span>|<span data-ttu-id="26ce5-p104">Representa o conjunto do qual o ícone faz parte. Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles` e `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="26ce5-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="26ce5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ce5-138">Response</span></span>

<span data-ttu-id="26ce5-139">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookIcon](../resources/workbookicon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ce5-139">If successful, this method returns a `200 OK` response code and updated [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26ce5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26ce5-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26ce5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26ce5-141">Request</span></span>
<span data-ttu-id="26ce5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ce5-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="26ce5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ce5-143">Response</span></span>
<span data-ttu-id="26ce5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26ce5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
