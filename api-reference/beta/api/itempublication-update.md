---
title: Atualizar itemPublication
description: Atualize as propriedades de um objeto itemPublication.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bf715534a5af58136f91b7567fa675d85c174696
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770358"
---
# <a name="update-itempublication"></a><span data-ttu-id="5b6bd-103">Atualizar itemPublication</span><span class="sxs-lookup"><span data-stu-id="5b6bd-103">Update itemPublication</span></span>

<span data-ttu-id="5b6bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b6bd-105">Atualize as propriedades de [um objeto itemPublication](../resources/itempublication.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5b6bd-105">Update the properties of an [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b6bd-106">Permissions</span></span>

<span data-ttu-id="5b6bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b6bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b6bd-109">Permission type</span></span>                        | <span data-ttu-id="5b6bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b6bd-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5b6bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b6bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b6bd-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b6bd-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5b6bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b6bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6bd-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b6bd-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5b6bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b6bd-115">Application</span></span>                            | <span data-ttu-id="5b6bd-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b6bd-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5b6bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6bd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/publications/{id}
PATCH /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5b6bd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6bd-118">Request headers</span></span>
|<span data-ttu-id="5b6bd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5b6bd-119">Name</span></span>|<span data-ttu-id="5b6bd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b6bd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b6bd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b6bd-121">Authorization</span></span>|<span data-ttu-id="5b6bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5b6bd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b6bd-124">Content-Type</span></span>|<span data-ttu-id="5b6bd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b6bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6bd-127">Request body</span></span>

<span data-ttu-id="5b6bd-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5b6bd-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b6bd-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="5b6bd-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b6bd-131">Property</span></span>|<span data-ttu-id="5b6bd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b6bd-132">Type</span></span>|<span data-ttu-id="5b6bd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b6bd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b6bd-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5b6bd-134">allowedAudiences</span></span>|<span data-ttu-id="5b6bd-135">String</span><span class="sxs-lookup"><span data-stu-id="5b6bd-135">String</span></span>|<span data-ttu-id="5b6bd-136">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5b6bd-137">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5b6bd-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5b6bd-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5b6bd-139">descrição</span><span class="sxs-lookup"><span data-stu-id="5b6bd-139">description</span></span>    |<span data-ttu-id="5b6bd-140">String</span><span class="sxs-lookup"><span data-stu-id="5b6bd-140">String</span></span>      |<span data-ttu-id="5b6bd-141">Descrição da publicação.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-141">Description of the publication.</span></span>                   |
|<span data-ttu-id="5b6bd-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5b6bd-142">displayName</span></span>    |<span data-ttu-id="5b6bd-143">String</span><span class="sxs-lookup"><span data-stu-id="5b6bd-143">String</span></span>      |<span data-ttu-id="5b6bd-144">Título da publicação.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-144">Title of the publication.</span></span>                         |
|<span data-ttu-id="5b6bd-145">inferência</span><span class="sxs-lookup"><span data-stu-id="5b6bd-145">inference</span></span>|[<span data-ttu-id="5b6bd-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5b6bd-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5b6bd-147">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5b6bd-148">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5b6bd-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5b6bd-149">publishedDate</span><span class="sxs-lookup"><span data-stu-id="5b6bd-149">publishedDate</span></span>  |<span data-ttu-id="5b6bd-150">Data</span><span class="sxs-lookup"><span data-stu-id="5b6bd-150">Date</span></span>        |<span data-ttu-id="5b6bd-151">A data em que a publicação foi publicada.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-151">The date that the publication was published.</span></span>      |
|<span data-ttu-id="5b6bd-152">publicador</span><span class="sxs-lookup"><span data-stu-id="5b6bd-152">publisher</span></span>      |<span data-ttu-id="5b6bd-153">String</span><span class="sxs-lookup"><span data-stu-id="5b6bd-153">String</span></span>      |<span data-ttu-id="5b6bd-154">Publicação ou Editor para a publicação.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-154">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="5b6bd-155">source</span><span class="sxs-lookup"><span data-stu-id="5b6bd-155">source</span></span>|[<span data-ttu-id="5b6bd-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="5b6bd-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5b6bd-157">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5b6bd-158">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5b6bd-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5b6bd-159">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="5b6bd-159">thumbnailUrl</span></span>   |<span data-ttu-id="5b6bd-160">String</span><span class="sxs-lookup"><span data-stu-id="5b6bd-160">String</span></span>      |<span data-ttu-id="5b6bd-161">URL fazendo referência a uma miniatura da publicação.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-161">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="5b6bd-162">webUrl</span><span class="sxs-lookup"><span data-stu-id="5b6bd-162">webUrl</span></span>         |<span data-ttu-id="5b6bd-163">String</span><span class="sxs-lookup"><span data-stu-id="5b6bd-163">String</span></span>      |<span data-ttu-id="5b6bd-164">URL fazendo referência à publicação.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-164">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="5b6bd-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6bd-165">Response</span></span>

<span data-ttu-id="5b6bd-166">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto itemPublication](../resources/itemPublication.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-166">If successful, this method returns a `200 OK` response code and an updated [itemPublication](../resources/itemPublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b6bd-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b6bd-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b6bd-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6bd-168">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="5b6bd-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6bd-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemPublication"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/publications/{id}
Content-Type: application/json
Content-length: 497

{
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
}
```
# <a name="c"></a>[<span data-ttu-id="5b6bd-170">C#</span><span class="sxs-lookup"><span data-stu-id="5b6bd-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itempublication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b6bd-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b6bd-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itempublication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b6bd-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b6bd-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itempublication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b6bd-173">Java</span><span class="sxs-lookup"><span data-stu-id="5b6bd-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-itempublication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5b6bd-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6bd-174">Response</span></span>
<span data-ttu-id="5b6bd-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5b6bd-175">**Note:** The response object shown here might be shortened for readability.</span></span>
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


