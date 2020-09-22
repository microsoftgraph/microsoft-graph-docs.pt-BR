---
title: Atualizar countryNamedlocation
description: Atualiza as propriedades de um objeto countryNamedLocation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08c702475388d55a4964d6eadd14a75e12394360
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002629"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="a8701-103">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="a8701-103">Update countryNamedLocation</span></span>

<span data-ttu-id="a8701-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8701-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8701-105">Atualiza as propriedades de um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="a8701-105">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8701-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8701-106">Permissions</span></span>

<span data-ttu-id="a8701-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8701-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8701-109">Permission type</span></span>                        | <span data-ttu-id="a8701-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8701-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8701-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8701-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8701-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="a8701-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="a8701-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8701-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8701-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8701-114">Not supported.</span></span> |
| <span data-ttu-id="a8701-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8701-115">Application</span></span>                            | <span data-ttu-id="a8701-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="a8701-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8701-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8701-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a8701-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8701-118">Request headers</span></span>

| <span data-ttu-id="a8701-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a8701-119">Name</span></span>       | <span data-ttu-id="a8701-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8701-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a8701-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8701-121">Authorization</span></span> | <span data-ttu-id="a8701-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8701-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8701-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a8701-124">Content-type</span></span>  | <span data-ttu-id="a8701-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8701-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8701-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8701-127">Request body</span></span>

<span data-ttu-id="a8701-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a8701-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a8701-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a8701-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a8701-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a8701-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a8701-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8701-131">Property</span></span>     | <span data-ttu-id="a8701-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8701-132">Type</span></span>        | <span data-ttu-id="a8701-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8701-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8701-134">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="a8701-134">countriesAndRegions</span></span>|<span data-ttu-id="a8701-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8701-135">String collection</span></span>|<span data-ttu-id="a8701-136">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="a8701-136">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="a8701-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a8701-137">displayName</span></span>|<span data-ttu-id="a8701-138">String</span><span class="sxs-lookup"><span data-stu-id="a8701-138">String</span></span>|<span data-ttu-id="a8701-139">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="a8701-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="a8701-140">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="a8701-140">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="a8701-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8701-141">Boolean</span></span>|<span data-ttu-id="a8701-142">O valor é `true` se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="a8701-142">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="a8701-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8701-143">Response</span></span>

<span data-ttu-id="a8701-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8701-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8701-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8701-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8701-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8701-147">Request</span></span>

<span data-ttu-id="a8701-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8701-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8701-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8701-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
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
# <a name="javascript"></a>[<span data-ttu-id="a8701-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8701-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8701-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8701-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a8701-152">C#</span><span class="sxs-lookup"><span data-stu-id="a8701-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8701-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8701-153">Response</span></span>

<span data-ttu-id="a8701-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8701-154">The following is an example of the response.</span></span>

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


