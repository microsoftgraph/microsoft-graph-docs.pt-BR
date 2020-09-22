---
title: Atualizar a multipública
description: Atualizar as propriedades de um objeto de multipúblico.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 407e110d3d2f0da3a130b973c2382849b1db40bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999318"
---
# <a name="update-itempublication"></a><span data-ttu-id="85131-103">Atualizar a multipública</span><span class="sxs-lookup"><span data-stu-id="85131-103">Update itemPublication</span></span>

<span data-ttu-id="85131-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85131-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85131-105">Atualizar as propriedades de um objeto de [multipública](../resources/itempublication.md) em um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="85131-105">Update the properties of an [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85131-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85131-106">Permissions</span></span>

<span data-ttu-id="85131-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85131-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85131-109">Permission type</span></span>                        | <span data-ttu-id="85131-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85131-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="85131-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85131-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85131-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85131-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="85131-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85131-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85131-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85131-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="85131-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85131-115">Application</span></span>                            | <span data-ttu-id="85131-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85131-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="85131-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85131-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/publications/{id}
PATCH /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85131-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85131-118">Request headers</span></span>
|<span data-ttu-id="85131-119">Nome</span><span class="sxs-lookup"><span data-stu-id="85131-119">Name</span></span>|<span data-ttu-id="85131-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="85131-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="85131-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85131-121">Authorization</span></span>|<span data-ttu-id="85131-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85131-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="85131-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85131-124">Content-Type</span></span>|<span data-ttu-id="85131-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85131-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85131-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85131-127">Request body</span></span>

<span data-ttu-id="85131-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="85131-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="85131-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="85131-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="85131-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="85131-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="85131-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85131-131">Property</span></span>|<span data-ttu-id="85131-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="85131-132">Type</span></span>|<span data-ttu-id="85131-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="85131-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85131-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="85131-134">allowedAudiences</span></span>|<span data-ttu-id="85131-135">String</span><span class="sxs-lookup"><span data-stu-id="85131-135">String</span></span>|<span data-ttu-id="85131-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="85131-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="85131-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="85131-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="85131-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="85131-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="85131-139">description</span><span class="sxs-lookup"><span data-stu-id="85131-139">description</span></span>    |<span data-ttu-id="85131-140">String</span><span class="sxs-lookup"><span data-stu-id="85131-140">String</span></span>      |<span data-ttu-id="85131-141">Descrição da publicação.</span><span class="sxs-lookup"><span data-stu-id="85131-141">Description of the publication.</span></span>                   |
|<span data-ttu-id="85131-142">displayName</span><span class="sxs-lookup"><span data-stu-id="85131-142">displayName</span></span>    |<span data-ttu-id="85131-143">String</span><span class="sxs-lookup"><span data-stu-id="85131-143">String</span></span>      |<span data-ttu-id="85131-144">Título da publicação.</span><span class="sxs-lookup"><span data-stu-id="85131-144">Title of the publication.</span></span>                         |
|<span data-ttu-id="85131-145">fracassa</span><span class="sxs-lookup"><span data-stu-id="85131-145">inference</span></span>|[<span data-ttu-id="85131-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="85131-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="85131-147">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="85131-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="85131-148">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="85131-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="85131-149">publishedDate</span><span class="sxs-lookup"><span data-stu-id="85131-149">publishedDate</span></span>  |<span data-ttu-id="85131-150">Data</span><span class="sxs-lookup"><span data-stu-id="85131-150">Date</span></span>        |<span data-ttu-id="85131-151">A data em que a publicação foi publicada.</span><span class="sxs-lookup"><span data-stu-id="85131-151">The date that the publication was published.</span></span>      |
|<span data-ttu-id="85131-152">publicador</span><span class="sxs-lookup"><span data-stu-id="85131-152">publisher</span></span>      |<span data-ttu-id="85131-153">String</span><span class="sxs-lookup"><span data-stu-id="85131-153">String</span></span>      |<span data-ttu-id="85131-154">Publicação ou editor para a publicação.</span><span class="sxs-lookup"><span data-stu-id="85131-154">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="85131-155">source</span><span class="sxs-lookup"><span data-stu-id="85131-155">source</span></span>|[<span data-ttu-id="85131-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="85131-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="85131-157">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="85131-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="85131-158">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="85131-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="85131-159">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="85131-159">thumbnailUrl</span></span>   |<span data-ttu-id="85131-160">String</span><span class="sxs-lookup"><span data-stu-id="85131-160">String</span></span>      |<span data-ttu-id="85131-161">URL que faz referência a uma miniatura da publicação.</span><span class="sxs-lookup"><span data-stu-id="85131-161">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="85131-162">webUrl</span><span class="sxs-lookup"><span data-stu-id="85131-162">webUrl</span></span>         |<span data-ttu-id="85131-163">String</span><span class="sxs-lookup"><span data-stu-id="85131-163">String</span></span>      |<span data-ttu-id="85131-164">URL que faz referência à publicação.</span><span class="sxs-lookup"><span data-stu-id="85131-164">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="85131-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="85131-165">Response</span></span>

<span data-ttu-id="85131-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [dopublication](../resources/itemPublication.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85131-166">If successful, this method returns a `200 OK` response code and an updated [itemPublication](../resources/itemPublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85131-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85131-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85131-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85131-168">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="85131-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="85131-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemPublication"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/publications/{id}
Content-Type: application/json
Content-length: 497

{
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
}
```
# <a name="c"></a>[<span data-ttu-id="85131-170">C#</span><span class="sxs-lookup"><span data-stu-id="85131-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85131-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85131-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85131-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85131-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="85131-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="85131-173">Response</span></span>
<span data-ttu-id="85131-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85131-174">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
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
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


