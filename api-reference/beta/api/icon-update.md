---
title: Atualizar ícone
description: Atualize as propriedades do objeto de ícone.
localization_priority: Normal
ms.openlocfilehash: 83e9845e87018a6f7b059a917643c1c51ccd01d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859175"
---
# <a name="update-icon"></a><span data-ttu-id="f1bf5-103">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="f1bf5-103">Update icon</span></span>

> <span data-ttu-id="f1bf5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1bf5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1bf5-106">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-106">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1bf5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1bf5-107">Permissions</span></span>
<span data-ttu-id="f1bf5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1bf5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1bf5-110">Permission type</span></span>      | <span data-ttu-id="f1bf5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1bf5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1bf5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1bf5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1bf5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1bf5-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1bf5-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1bf5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1bf5-116">Application</span></span> | <span data-ttu-id="f1bf5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1bf5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1bf5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="f1bf5-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f1bf5-119">Optional request headers</span></span>
| <span data-ttu-id="f1bf5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f1bf5-120">Name</span></span>       | <span data-ttu-id="f1bf5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1bf5-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1bf5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1bf5-122">Authorization</span></span>  | <span data-ttu-id="f1bf5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1bf5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bf5-125">Request body</span></span>
<span data-ttu-id="f1bf5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1bf5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1bf5-129">Property</span></span>     | <span data-ttu-id="f1bf5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1bf5-130">Type</span></span>   |<span data-ttu-id="f1bf5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1bf5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1bf5-132">índice</span><span class="sxs-lookup"><span data-stu-id="f1bf5-132">index</span></span>|<span data-ttu-id="f1bf5-133">int</span><span class="sxs-lookup"><span data-stu-id="f1bf5-133">int</span></span>|<span data-ttu-id="f1bf5-134">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-134">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="f1bf5-135">set</span><span class="sxs-lookup"><span data-stu-id="f1bf5-135">set</span></span>|<span data-ttu-id="f1bf5-136">string</span><span class="sxs-lookup"><span data-stu-id="f1bf5-136">string</span></span>|<span data-ttu-id="f1bf5-p105">Representa o conjunto do qual o ícone faz parte. Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles` e `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p105">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="f1bf5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1bf5-139">Response</span></span>

<span data-ttu-id="f1bf5-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Icon](../resources/icon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-140">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1bf5-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1bf5-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1bf5-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bf5-142">Request</span></span>
<span data-ttu-id="f1bf5-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f1bf5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1bf5-144">Response</span></span>
<span data-ttu-id="f1bf5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
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
