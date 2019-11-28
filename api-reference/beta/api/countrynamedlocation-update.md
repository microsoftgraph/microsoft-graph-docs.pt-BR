---
title: Atualizar countryNamedlocation
description: Atualiza as propriedades de um objeto countryNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81224b2c0e31ad4ade9caeca661624e1b0fe4383
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636740"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="27f51-103">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="27f51-103">Update countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27f51-104">Atualiza as propriedades de um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="27f51-104">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27f51-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27f51-105">Permissions</span></span>

<span data-ttu-id="27f51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27f51-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27f51-108">Permission type</span></span>                        | <span data-ttu-id="27f51-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27f51-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27f51-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27f51-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27f51-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="27f51-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="27f51-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27f51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27f51-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f51-113">Not supported.</span></span> |
| <span data-ttu-id="27f51-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27f51-114">Application</span></span>                            | <span data-ttu-id="27f51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f51-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27f51-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27f51-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27f51-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27f51-117">Request headers</span></span>

| <span data-ttu-id="27f51-118">Nome</span><span class="sxs-lookup"><span data-stu-id="27f51-118">Name</span></span>       | <span data-ttu-id="27f51-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="27f51-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="27f51-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="27f51-120">Authorization</span></span> | <span data-ttu-id="27f51-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27f51-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27f51-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="27f51-123">Content-type</span></span>  | <span data-ttu-id="27f51-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27f51-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27f51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27f51-126">Request body</span></span>

<span data-ttu-id="27f51-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="27f51-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="27f51-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="27f51-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="27f51-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="27f51-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="27f51-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27f51-130">Property</span></span>     | <span data-ttu-id="27f51-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27f51-131">Type</span></span>        | <span data-ttu-id="27f51-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27f51-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27f51-133">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="27f51-133">countriesAndRegions</span></span>|<span data-ttu-id="27f51-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="27f51-134">String collection</span></span>|<span data-ttu-id="27f51-135">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="27f51-135">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="27f51-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27f51-136">displayName</span></span>|<span data-ttu-id="27f51-137">String</span><span class="sxs-lookup"><span data-stu-id="27f51-137">String</span></span>|<span data-ttu-id="27f51-138">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="27f51-138">Human-readable name of the location.</span></span>|
|<span data-ttu-id="27f51-139">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="27f51-139">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="27f51-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="27f51-140">Boolean</span></span>|<span data-ttu-id="27f51-141">O valor é `true` se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="27f51-141">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="27f51-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f51-142">Response</span></span>

<span data-ttu-id="27f51-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27f51-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27f51-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27f51-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27f51-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27f51-146">Request</span></span>

<span data-ttu-id="27f51-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27f51-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27f51-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="27f51-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Updated named location without unknown countries and regions",
    "countriesAndRegions": [
        "CA",
        "IN"
    ],
    "includeUnknownCountriesAndRegions": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27f51-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27f51-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27f51-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27f51-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27f51-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f51-151">Response</span></span>

<span data-ttu-id="27f51-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27f51-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update countrynamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
