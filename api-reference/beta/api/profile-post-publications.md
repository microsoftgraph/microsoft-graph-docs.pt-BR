---
title: Criar publicações
description: Criar um novo objeto publications.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6e6992fa3bd871a3e80c7c9a949461d788e6926f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034361"
---
# <a name="create-itempublication"></a><span data-ttu-id="64fb7-103">Criar a multipúblico</span><span class="sxs-lookup"><span data-stu-id="64fb7-103">Create itemPublication</span></span>
<span data-ttu-id="64fb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64fb7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64fb7-105">Criar um novo objeto [Dopublication](../resources/itempublication.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="64fb7-105">Create a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64fb7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64fb7-106">Permissions</span></span>

<span data-ttu-id="64fb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64fb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64fb7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64fb7-109">Permission type</span></span>                        | <span data-ttu-id="64fb7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64fb7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="64fb7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64fb7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64fb7-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="64fb7-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="64fb7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64fb7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fb7-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="64fb7-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="64fb7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64fb7-115">Application</span></span>                            | <span data-ttu-id="64fb7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fb7-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="64fb7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a><span data-ttu-id="64fb7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb7-118">Request headers</span></span>
|<span data-ttu-id="64fb7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="64fb7-119">Name</span></span>|<span data-ttu-id="64fb7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="64fb7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64fb7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64fb7-121">Authorization</span></span>|<span data-ttu-id="64fb7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64fb7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="64fb7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64fb7-124">Content-Type</span></span>|<span data-ttu-id="64fb7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64fb7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64fb7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb7-127">Request body</span></span>
<span data-ttu-id="64fb7-128">No corpo da solicitação, forneça uma representação JSON do objeto [Dopublication](../resources/itempublication.md) .</span><span class="sxs-lookup"><span data-stu-id="64fb7-128">In the request body, supply a JSON representation of the [itemPublication](../resources/itempublication.md) object.</span></span>

<span data-ttu-id="64fb7-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto de [multipúblico](../resources/itempublication.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="64fb7-129">The following table shows the properties that are possible to set when creating a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="64fb7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64fb7-130">Property</span></span>|<span data-ttu-id="64fb7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="64fb7-131">Type</span></span>|<span data-ttu-id="64fb7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="64fb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64fb7-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="64fb7-133">allowedAudiences</span></span>|<span data-ttu-id="64fb7-134">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-134">String</span></span>|<span data-ttu-id="64fb7-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="64fb7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="64fb7-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="64fb7-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="64fb7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="64fb7-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="64fb7-138">createdBy</span></span>|[<span data-ttu-id="64fb7-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="64fb7-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="64fb7-140">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="64fb7-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="64fb7-141">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="64fb7-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64fb7-142">createdDateTime</span></span>|<span data-ttu-id="64fb7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64fb7-143">DateTimeOffset</span></span>|<span data-ttu-id="64fb7-144">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="64fb7-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="64fb7-145">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="64fb7-146">description</span><span class="sxs-lookup"><span data-stu-id="64fb7-146">description</span></span>    |<span data-ttu-id="64fb7-147">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-147">String</span></span>      |<span data-ttu-id="64fb7-148">Descrição da publicação.</span><span class="sxs-lookup"><span data-stu-id="64fb7-148">Description of the publication.</span></span>                   |
|<span data-ttu-id="64fb7-149">displayName</span><span class="sxs-lookup"><span data-stu-id="64fb7-149">displayName</span></span>    |<span data-ttu-id="64fb7-150">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-150">String</span></span>      |<span data-ttu-id="64fb7-151">Título da publicação.</span><span class="sxs-lookup"><span data-stu-id="64fb7-151">Title of the publication.</span></span>                         |
|<span data-ttu-id="64fb7-152">id</span><span class="sxs-lookup"><span data-stu-id="64fb7-152">id</span></span>|<span data-ttu-id="64fb7-153">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-153">String</span></span>|<span data-ttu-id="64fb7-154">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="64fb7-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="64fb7-155">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="64fb7-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="64fb7-156">fracassa</span><span class="sxs-lookup"><span data-stu-id="64fb7-156">inference</span></span>|[<span data-ttu-id="64fb7-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="64fb7-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="64fb7-158">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="64fb7-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="64fb7-159">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="64fb7-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="64fb7-160">lastModifiedBy</span></span>|[<span data-ttu-id="64fb7-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="64fb7-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="64fb7-162">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="64fb7-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="64fb7-163">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="64fb7-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64fb7-164">lastModifiedDateTime</span></span>|<span data-ttu-id="64fb7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64fb7-165">DateTimeOffset</span></span>|<span data-ttu-id="64fb7-166">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="64fb7-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="64fb7-167">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="64fb7-168">publishedDate</span><span class="sxs-lookup"><span data-stu-id="64fb7-168">publishedDate</span></span>  |<span data-ttu-id="64fb7-169">Data</span><span class="sxs-lookup"><span data-stu-id="64fb7-169">Date</span></span>        |<span data-ttu-id="64fb7-170">A data em que a publicação foi publicada.</span><span class="sxs-lookup"><span data-stu-id="64fb7-170">The date that the publication was published.</span></span>      |
|<span data-ttu-id="64fb7-171">publicador</span><span class="sxs-lookup"><span data-stu-id="64fb7-171">publisher</span></span>      |<span data-ttu-id="64fb7-172">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-172">String</span></span>      |<span data-ttu-id="64fb7-173">Publicação ou editor para a publicação.</span><span class="sxs-lookup"><span data-stu-id="64fb7-173">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="64fb7-174">source</span><span class="sxs-lookup"><span data-stu-id="64fb7-174">source</span></span>|[<span data-ttu-id="64fb7-175">personDataSource</span><span class="sxs-lookup"><span data-stu-id="64fb7-175">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="64fb7-176">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="64fb7-176">Where the values originated if synced from another service.</span></span> <span data-ttu-id="64fb7-177">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-177">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="64fb7-178">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="64fb7-178">thumbnailUrl</span></span>   |<span data-ttu-id="64fb7-179">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-179">String</span></span>      |<span data-ttu-id="64fb7-180">URL que faz referência a uma miniatura da publicação.</span><span class="sxs-lookup"><span data-stu-id="64fb7-180">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="64fb7-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="64fb7-181">webUrl</span></span>         |<span data-ttu-id="64fb7-182">String</span><span class="sxs-lookup"><span data-stu-id="64fb7-182">String</span></span>      |<span data-ttu-id="64fb7-183">URL que faz referência à publicação.</span><span class="sxs-lookup"><span data-stu-id="64fb7-183">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="64fb7-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb7-184">Response</span></span>

<span data-ttu-id="64fb7-185">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [dopublication](../resources/itempublication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64fb7-185">If successful, this method returns a `201 Created` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64fb7-186">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64fb7-186">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="64fb7-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb7-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemPublication_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/publications
Content-Type: application/json
Content-length: 497

{
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="64fb7-188">C#</span><span class="sxs-lookup"><span data-stu-id="64fb7-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64fb7-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64fb7-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64fb7-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64fb7-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="64fb7-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb7-191">Response</span></span>
<span data-ttu-id="64fb7-192">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64fb7-192">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
}
-->
``` http
HTTP/1.1 201 Created
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


