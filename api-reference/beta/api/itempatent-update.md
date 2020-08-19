---
title: Atualizar a ispatente
description: Atualiza as propriedades de um objeto dopatente.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 29181e23833bb60d8722d3f82aaec44eafd5ad35
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809587"
---
# <a name="update-itempatent"></a><span data-ttu-id="e8dbd-103">Atualizar a ispatente</span><span class="sxs-lookup"><span data-stu-id="e8dbd-103">Update itemPatent</span></span>

<span data-ttu-id="e8dbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8dbd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8dbd-105">Atualiza as propriedades de um objeto [dopatente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="e8dbd-105">Update the properties of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8dbd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8dbd-106">Permissions</span></span>

<span data-ttu-id="e8dbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8dbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8dbd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8dbd-109">Permission type</span></span>                        | <span data-ttu-id="e8dbd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8dbd-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e8dbd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8dbd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8dbd-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8dbd-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e8dbd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8dbd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8dbd-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8dbd-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e8dbd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8dbd-115">Application</span></span>                            | <span data-ttu-id="e8dbd-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8dbd-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e8dbd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8dbd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/patents/{id}
PATCH /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8dbd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8dbd-118">Request headers</span></span>
|<span data-ttu-id="e8dbd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e8dbd-119">Name</span></span>|<span data-ttu-id="e8dbd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8dbd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8dbd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8dbd-121">Authorization</span></span>|<span data-ttu-id="e8dbd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e8dbd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8dbd-124">Content-Type</span></span>|<span data-ttu-id="e8dbd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8dbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8dbd-127">Request body</span></span>

<span data-ttu-id="e8dbd-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e8dbd-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e8dbd-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="e8dbd-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8dbd-131">Property</span></span>|<span data-ttu-id="e8dbd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8dbd-132">Type</span></span>|<span data-ttu-id="e8dbd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8dbd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8dbd-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e8dbd-134">allowedAudiences</span></span>|<span data-ttu-id="e8dbd-135">String</span><span class="sxs-lookup"><span data-stu-id="e8dbd-135">String</span></span>|<span data-ttu-id="e8dbd-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e8dbd-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e8dbd-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e8dbd-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e8dbd-139">description</span><span class="sxs-lookup"><span data-stu-id="e8dbd-139">description</span></span>|<span data-ttu-id="e8dbd-140">String</span><span class="sxs-lookup"><span data-stu-id="e8dbd-140">String</span></span>|<span data-ttu-id="e8dbd-141">Descpription da patente ou do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-141">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="e8dbd-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e8dbd-142">displayName</span></span>|<span data-ttu-id="e8dbd-143">String</span><span class="sxs-lookup"><span data-stu-id="e8dbd-143">String</span></span>|<span data-ttu-id="e8dbd-144">Título da patente ou do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-144">Title of the patent or filing.</span></span> |
|<span data-ttu-id="e8dbd-145">fracassa</span><span class="sxs-lookup"><span data-stu-id="e8dbd-145">inference</span></span>|[<span data-ttu-id="e8dbd-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e8dbd-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e8dbd-147">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e8dbd-148">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e8dbd-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e8dbd-149">ispending</span><span class="sxs-lookup"><span data-stu-id="e8dbd-149">isPending</span></span>        |<span data-ttu-id="e8dbd-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8dbd-150">Boolean</span></span>     |<span data-ttu-id="e8dbd-151">Indica que a patente está pendente.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-151">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="e8dbd-152">issuedDate</span><span class="sxs-lookup"><span data-stu-id="e8dbd-152">issuedDate</span></span>       |<span data-ttu-id="e8dbd-153">Data</span><span class="sxs-lookup"><span data-stu-id="e8dbd-153">Date</span></span>        |<span data-ttu-id="e8dbd-154">A data em que a patente foi concedida.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-154">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="e8dbd-155">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="e8dbd-155">issuingAuthority</span></span> |<span data-ttu-id="e8dbd-156">String</span><span class="sxs-lookup"><span data-stu-id="e8dbd-156">String</span></span>      |<span data-ttu-id="e8dbd-157">Autoridade que concedeu a patente.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-157">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="e8dbd-158">number</span><span class="sxs-lookup"><span data-stu-id="e8dbd-158">number</span></span>           |<span data-ttu-id="e8dbd-159">String</span><span class="sxs-lookup"><span data-stu-id="e8dbd-159">String</span></span>      |<span data-ttu-id="e8dbd-160">O número de patente.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-160">The patent number.</span></span>                      |
|<span data-ttu-id="e8dbd-161">source</span><span class="sxs-lookup"><span data-stu-id="e8dbd-161">source</span></span>|[<span data-ttu-id="e8dbd-162">personDataSource</span><span class="sxs-lookup"><span data-stu-id="e8dbd-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e8dbd-163">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e8dbd-164">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e8dbd-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e8dbd-165">webUrl</span><span class="sxs-lookup"><span data-stu-id="e8dbd-165">webUrl</span></span>           |<span data-ttu-id="e8dbd-166">String</span><span class="sxs-lookup"><span data-stu-id="e8dbd-166">String</span></span>      |<span data-ttu-id="e8dbd-167">URL que faz referência à patente ou ao arquivamento.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-167">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="e8dbd-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8dbd-168">Response</span></span>

<span data-ttu-id="e8dbd-169">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [multipatente](../resources/itempatent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-169">If successful, this method returns a `200 OK` response code and an updated [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8dbd-170">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8dbd-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8dbd-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8dbd-171">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="e8dbd-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8dbd-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itempatent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/patents/{id}
Content-Type: application/json
Content-length: 497

{
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="e8dbd-173">C#</span><span class="sxs-lookup"><span data-stu-id="e8dbd-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8dbd-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8dbd-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8dbd-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8dbd-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e8dbd-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8dbd-176">Response</span></span>
<span data-ttu-id="e8dbd-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8dbd-177">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
