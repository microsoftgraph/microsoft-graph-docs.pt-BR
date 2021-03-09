---
title: Atualizar itemAddress
description: Atualize as propriedades de um objeto itemAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f53f5ad68919898dc337ed9b7c0f106ed3fa6c41
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578693"
---
# <a name="update-itemaddress"></a><span data-ttu-id="ba26d-103">Atualizar itemAddress</span><span class="sxs-lookup"><span data-stu-id="ba26d-103">Update itemAddress</span></span>
<span data-ttu-id="ba26d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba26d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba26d-105">Atualize as propriedades de um [objeto itemAddress.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="ba26d-105">Update the properties of an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba26d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba26d-106">Permissions</span></span>

<span data-ttu-id="ba26d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba26d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba26d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba26d-109">Permission type</span></span>                        | <span data-ttu-id="ba26d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba26d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ba26d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba26d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba26d-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba26d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ba26d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba26d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba26d-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba26d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ba26d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba26d-115">Application</span></span>                            | <span data-ttu-id="ba26d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba26d-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ba26d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba26d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/addresses/{id}
PATCH /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba26d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba26d-118">Request headers</span></span>
|<span data-ttu-id="ba26d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ba26d-119">Name</span></span>|<span data-ttu-id="ba26d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba26d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba26d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba26d-121">Authorization</span></span>|<span data-ttu-id="ba26d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba26d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ba26d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba26d-124">Content-Type</span></span>|<span data-ttu-id="ba26d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba26d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba26d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba26d-127">Request body</span></span>

<span data-ttu-id="ba26d-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ba26d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ba26d-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ba26d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ba26d-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ba26d-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="ba26d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba26d-131">Property</span></span>|<span data-ttu-id="ba26d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba26d-132">Type</span></span>|<span data-ttu-id="ba26d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba26d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba26d-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ba26d-134">allowedAudiences</span></span>|<span data-ttu-id="ba26d-135">String</span><span class="sxs-lookup"><span data-stu-id="ba26d-135">String</span></span>|<span data-ttu-id="ba26d-136">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="ba26d-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ba26d-137">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ba26d-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ba26d-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ba26d-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ba26d-139">detail</span><span class="sxs-lookup"><span data-stu-id="ba26d-139">detail</span></span>|[<span data-ttu-id="ba26d-140">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="ba26d-140">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="ba26d-141">Detalhes sobre o endereço em si.</span><span class="sxs-lookup"><span data-stu-id="ba26d-141">Details about the address itself.</span></span>|
|<span data-ttu-id="ba26d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ba26d-142">displayName</span></span>|<span data-ttu-id="ba26d-143">String</span><span class="sxs-lookup"><span data-stu-id="ba26d-143">String</span></span>|<span data-ttu-id="ba26d-144">Nome amigável que o usuário atribuiu a esse endereço.</span><span class="sxs-lookup"><span data-stu-id="ba26d-144">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="ba26d-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="ba26d-145">geoCoordinates</span></span>|[<span data-ttu-id="ba26d-146">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="ba26d-146">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="ba26d-147">As geocoordinações do endereço.</span><span class="sxs-lookup"><span data-stu-id="ba26d-147">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="ba26d-148">inferência</span><span class="sxs-lookup"><span data-stu-id="ba26d-148">inference</span></span>|[<span data-ttu-id="ba26d-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ba26d-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ba26d-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="ba26d-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ba26d-151">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ba26d-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ba26d-152">source</span><span class="sxs-lookup"><span data-stu-id="ba26d-152">source</span></span>|[<span data-ttu-id="ba26d-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="ba26d-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ba26d-154">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="ba26d-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ba26d-155">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ba26d-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ba26d-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba26d-156">Response</span></span>

<span data-ttu-id="ba26d-157">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto itemAddress](../resources/itemaddress.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba26d-157">If successful, this method returns a `200 OK` response code and an updated [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba26d-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba26d-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba26d-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba26d-159">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="ba26d-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba26d-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemaddress"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
Content-Type: application/json
Content-length: 497

{
  "allowedAudiences": "me",
  "displayName": "Secret Hideout",
}
```
# <a name="c"></a>[<span data-ttu-id="ba26d-161">C#</span><span class="sxs-lookup"><span data-stu-id="ba26d-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba26d-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba26d-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba26d-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba26d-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ba26d-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba26d-164">Response</span></span>
<span data-ttu-id="ba26d-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba26d-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "displayName": "Secret Hideout",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  },
  "geoCoordinates": null
}
```



