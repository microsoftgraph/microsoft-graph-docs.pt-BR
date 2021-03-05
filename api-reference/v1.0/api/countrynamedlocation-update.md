---
title: Atualizar countryNamedlocation
description: Atualize as propriedades de um objeto countryNamedLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fa684d1dc42887f636217056e30e5a0807507bef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434671"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="eb349-103">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb349-103">Update countryNamedLocation</span></span>

<span data-ttu-id="eb349-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb349-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb349-105">Atualize as propriedades de um [objeto countryNamedLocation.](../resources/countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="eb349-105">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb349-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb349-106">Permissions</span></span>

<span data-ttu-id="eb349-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb349-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb349-109">Permission type</span></span>                        | <span data-ttu-id="eb349-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb349-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eb349-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb349-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb349-112">Policy.Read.All e Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="eb349-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="eb349-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb349-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb349-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb349-114">Not supported.</span></span> |
| <span data-ttu-id="eb349-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb349-115">Application</span></span>                            | <span data-ttu-id="eb349-116">Policy.Read.All e Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="eb349-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb349-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb349-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eb349-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb349-118">Request headers</span></span>

| <span data-ttu-id="eb349-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eb349-119">Name</span></span>       | <span data-ttu-id="eb349-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb349-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eb349-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb349-121">Authorization</span></span> | <span data-ttu-id="eb349-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb349-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb349-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="eb349-124">Content-type</span></span>  | <span data-ttu-id="eb349-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb349-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb349-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb349-127">Request body</span></span>

<span data-ttu-id="eb349-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="eb349-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eb349-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="eb349-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eb349-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eb349-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eb349-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb349-131">Property</span></span>     | <span data-ttu-id="eb349-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb349-132">Type</span></span>        | <span data-ttu-id="eb349-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb349-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb349-134">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="eb349-134">countriesAndRegions</span></span>|<span data-ttu-id="eb349-135">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb349-135">String collection</span></span>|<span data-ttu-id="eb349-136">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="eb349-136">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="eb349-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eb349-137">displayName</span></span>|<span data-ttu-id="eb349-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb349-138">String</span></span>|<span data-ttu-id="eb349-139">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="eb349-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="eb349-140">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="eb349-140">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="eb349-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb349-141">Boolean</span></span>|<span data-ttu-id="eb349-142">O valor é `true` se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="eb349-142">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="eb349-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb349-143">Response</span></span>

<span data-ttu-id="eb349-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb349-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb349-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb349-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb349-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb349-147">Request</span></span>

<span data-ttu-id="eb349-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb349-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb349-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb349-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
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
# <a name="c"></a>[<span data-ttu-id="eb349-150">C#</span><span class="sxs-lookup"><span data-stu-id="eb349-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb349-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb349-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb349-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb349-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb349-153">Java</span><span class="sxs-lookup"><span data-stu-id="eb349-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb349-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb349-154">Response</span></span>

<span data-ttu-id="eb349-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb349-155">The following is an example of the response.</span></span>

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

