---
title: Criar prêmios
description: Criar um novo objeto de prêmios.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c7745c6b31678bfbf793a0897edcfb6606953d42
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964541"
---
# <a name="create-personaward"></a><span data-ttu-id="71cdb-103">Criar personAward</span><span class="sxs-lookup"><span data-stu-id="71cdb-103">Create personAward</span></span>

<span data-ttu-id="71cdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71cdb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71cdb-105">Criar um novo objeto [personAward](../resources/personaward.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="71cdb-105">Create a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71cdb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71cdb-106">Permissions</span></span>

<span data-ttu-id="71cdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71cdb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71cdb-109">Permission type</span></span>                        | <span data-ttu-id="71cdb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71cdb-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="71cdb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71cdb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71cdb-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="71cdb-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="71cdb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71cdb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71cdb-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="71cdb-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="71cdb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71cdb-115">Application</span></span>                            | <span data-ttu-id="71cdb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71cdb-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="71cdb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71cdb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/awards
POST /users/{id | userPrincipalName}/profile/awards
```

## <a name="request-headers"></a><span data-ttu-id="71cdb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71cdb-118">Request headers</span></span>
|<span data-ttu-id="71cdb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="71cdb-119">Name</span></span>|<span data-ttu-id="71cdb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="71cdb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71cdb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="71cdb-121">Authorization</span></span>|<span data-ttu-id="71cdb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71cdb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="71cdb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71cdb-124">Content-Type</span></span>|<span data-ttu-id="71cdb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71cdb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71cdb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71cdb-127">Request body</span></span>
<span data-ttu-id="71cdb-128">No corpo da solicitação, forneça uma representação JSON do objeto [personAward](../resources/personaward.md) .</span><span class="sxs-lookup"><span data-stu-id="71cdb-128">In the request body, supply a JSON representation of the [personAward](../resources/personaward.md) object.</span></span>

<span data-ttu-id="71cdb-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto [personAward](../resources/personaward.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="71cdb-129">The following table shows the properties that are possible to set when creating a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="71cdb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71cdb-130">Property</span></span>|<span data-ttu-id="71cdb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71cdb-131">Type</span></span>|<span data-ttu-id="71cdb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71cdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71cdb-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="71cdb-133">allowedAudiences</span></span>|<span data-ttu-id="71cdb-134">String</span><span class="sxs-lookup"><span data-stu-id="71cdb-134">String</span></span>|<span data-ttu-id="71cdb-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="71cdb-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="71cdb-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="71cdb-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="71cdb-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="71cdb-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="71cdb-138">description</span><span class="sxs-lookup"><span data-stu-id="71cdb-138">description</span></span>|<span data-ttu-id="71cdb-139">String</span><span class="sxs-lookup"><span data-stu-id="71cdb-139">String</span></span>|<span data-ttu-id="71cdb-140">Descpription do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="71cdb-140">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="71cdb-141">displayName</span><span class="sxs-lookup"><span data-stu-id="71cdb-141">displayName</span></span>|<span data-ttu-id="71cdb-142">String</span><span class="sxs-lookup"><span data-stu-id="71cdb-142">String</span></span>|<span data-ttu-id="71cdb-143">Nome do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="71cdb-143">Name of the award or honor.</span></span> |
|<span data-ttu-id="71cdb-144">fracassa</span><span class="sxs-lookup"><span data-stu-id="71cdb-144">inference</span></span>|[<span data-ttu-id="71cdb-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="71cdb-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="71cdb-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="71cdb-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="71cdb-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="71cdb-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="71cdb-148">issuedDate</span><span class="sxs-lookup"><span data-stu-id="71cdb-148">issuedDate</span></span>|<span data-ttu-id="71cdb-149">Data</span><span class="sxs-lookup"><span data-stu-id="71cdb-149">Date</span></span>|<span data-ttu-id="71cdb-150">A data em que o prêmio ou honra foi concedido.</span><span class="sxs-lookup"><span data-stu-id="71cdb-150">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="71cdb-151">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="71cdb-151">issuingAuthority</span></span>|<span data-ttu-id="71cdb-152">String</span><span class="sxs-lookup"><span data-stu-id="71cdb-152">String</span></span>|<span data-ttu-id="71cdb-153">Autoridade que concedeu o prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="71cdb-153">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="71cdb-154">source</span><span class="sxs-lookup"><span data-stu-id="71cdb-154">source</span></span>|[<span data-ttu-id="71cdb-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="71cdb-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="71cdb-156">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="71cdb-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="71cdb-157">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="71cdb-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="71cdb-158">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="71cdb-158">thumbnailUrl</span></span>|<span data-ttu-id="71cdb-159">String</span><span class="sxs-lookup"><span data-stu-id="71cdb-159">String</span></span>|<span data-ttu-id="71cdb-160">URL que faz referência a uma miniatura do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="71cdb-160">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="71cdb-161">webUrl</span><span class="sxs-lookup"><span data-stu-id="71cdb-161">webUrl</span></span>|<span data-ttu-id="71cdb-162">String</span><span class="sxs-lookup"><span data-stu-id="71cdb-162">String</span></span>|<span data-ttu-id="71cdb-163">URL que faz referência ao prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="71cdb-163">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="71cdb-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cdb-164">Response</span></span>

<span data-ttu-id="71cdb-165">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personAward](../resources/personaward.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71cdb-165">If successful, this method returns a `201 Created` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71cdb-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71cdb-166">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="71cdb-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="71cdb-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personaward_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/awards
Content-Type: application/json
Content-length: 497

{
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="71cdb-168">C#</span><span class="sxs-lookup"><span data-stu-id="71cdb-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personaward-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71cdb-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71cdb-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personaward-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71cdb-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71cdb-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personaward-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71cdb-171">Java</span><span class="sxs-lookup"><span data-stu-id="71cdb-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personaward-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="71cdb-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cdb-172">Response</span></span>
<span data-ttu-id="71cdb-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="71cdb-173">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


