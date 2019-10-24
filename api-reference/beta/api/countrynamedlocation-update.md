---
title: Atualizar countryNamedlocation
description: Atualiza as propriedades de um objeto countryNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d68138088ed39d8c4fe4dfbcec7abcb77aa11dd3
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653738"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="81a94-103">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="81a94-103">Update countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a94-104">Atualiza as propriedades de um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="81a94-104">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81a94-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="81a94-105">Permissions</span></span>

<span data-ttu-id="81a94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81a94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81a94-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81a94-108">Permission type</span></span>                        | <span data-ttu-id="81a94-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81a94-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81a94-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81a94-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81a94-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="81a94-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="81a94-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81a94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81a94-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a94-113">Not supported.</span></span> |
| <span data-ttu-id="81a94-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81a94-114">Application</span></span>                            | <span data-ttu-id="81a94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a94-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="81a94-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="81a94-116">This API requires multiple permissions.</span></span> <span data-ttu-id="81a94-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="81a94-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="81a94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81a94-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="81a94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81a94-119">Request headers</span></span>

| <span data-ttu-id="81a94-120">Nome</span><span class="sxs-lookup"><span data-stu-id="81a94-120">Name</span></span>       | <span data-ttu-id="81a94-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a94-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="81a94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81a94-122">Authorization</span></span> | <span data-ttu-id="81a94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a94-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81a94-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="81a94-125">Content-type</span></span>  | <span data-ttu-id="81a94-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a94-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81a94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81a94-128">Request body</span></span>

<span data-ttu-id="81a94-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="81a94-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="81a94-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="81a94-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="81a94-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="81a94-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="81a94-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81a94-132">Property</span></span>     | <span data-ttu-id="81a94-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="81a94-133">Type</span></span>        | <span data-ttu-id="81a94-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a94-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81a94-135">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="81a94-135">countriesAndRegions</span></span>|<span data-ttu-id="81a94-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="81a94-136">String collection</span></span>|<span data-ttu-id="81a94-137">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="81a94-137">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="81a94-138">displayName</span><span class="sxs-lookup"><span data-stu-id="81a94-138">displayName</span></span>|<span data-ttu-id="81a94-139">String</span><span class="sxs-lookup"><span data-stu-id="81a94-139">String</span></span>|<span data-ttu-id="81a94-140">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="81a94-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="81a94-141">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="81a94-141">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="81a94-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="81a94-142">Boolean</span></span>|<span data-ttu-id="81a94-143">O valor é `true` se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="81a94-143">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="81a94-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a94-144">Response</span></span>

<span data-ttu-id="81a94-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81a94-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81a94-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81a94-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81a94-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81a94-148">Request</span></span>

<span data-ttu-id="81a94-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81a94-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="81a94-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a94-150">Response</span></span>

<span data-ttu-id="81a94-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81a94-151">The following is an example of the response.</span></span>

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
