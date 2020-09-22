---
title: Criar prêmios
description: Criar um novo objeto de prêmios.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0ab51df665b9114bc590199319073efd90b5385e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034508"
---
# <a name="create-personaward"></a><span data-ttu-id="fece8-103">Criar personAward</span><span class="sxs-lookup"><span data-stu-id="fece8-103">Create personAward</span></span>

<span data-ttu-id="fece8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fece8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fece8-105">Criar um novo objeto [personAward](../resources/personaward.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fece8-105">Create a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fece8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fece8-106">Permissions</span></span>

<span data-ttu-id="fece8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fece8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fece8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fece8-109">Permission type</span></span>                        | <span data-ttu-id="fece8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fece8-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="fece8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fece8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fece8-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fece8-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fece8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fece8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fece8-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fece8-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fece8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fece8-115">Application</span></span>                            | <span data-ttu-id="fece8-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fece8-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="fece8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fece8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/awards
POST /users/{id | userPrincipalName}/profile/awards
```

## <a name="request-headers"></a><span data-ttu-id="fece8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fece8-118">Request headers</span></span>
|<span data-ttu-id="fece8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fece8-119">Name</span></span>|<span data-ttu-id="fece8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fece8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fece8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fece8-121">Authorization</span></span>|<span data-ttu-id="fece8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fece8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fece8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fece8-124">Content-Type</span></span>|<span data-ttu-id="fece8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fece8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fece8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fece8-127">Request body</span></span>
<span data-ttu-id="fece8-128">No corpo da solicitação, forneça uma representação JSON do objeto [personAward](../resources/personaward.md) .</span><span class="sxs-lookup"><span data-stu-id="fece8-128">In the request body, supply a JSON representation of the [personAward](../resources/personaward.md) object.</span></span>

<span data-ttu-id="fece8-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto [personAward](../resources/personaward.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fece8-129">The following table shows the properties that are possible to set when creating a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="fece8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fece8-130">Property</span></span>|<span data-ttu-id="fece8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fece8-131">Type</span></span>|<span data-ttu-id="fece8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fece8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fece8-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="fece8-133">allowedAudiences</span></span>|<span data-ttu-id="fece8-134">String</span><span class="sxs-lookup"><span data-stu-id="fece8-134">String</span></span>|<span data-ttu-id="fece8-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="fece8-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="fece8-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fece8-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="fece8-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fece8-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fece8-138">description</span><span class="sxs-lookup"><span data-stu-id="fece8-138">description</span></span>|<span data-ttu-id="fece8-139">String</span><span class="sxs-lookup"><span data-stu-id="fece8-139">String</span></span>|<span data-ttu-id="fece8-140">Descpription do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="fece8-140">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="fece8-141">displayName</span><span class="sxs-lookup"><span data-stu-id="fece8-141">displayName</span></span>|<span data-ttu-id="fece8-142">String</span><span class="sxs-lookup"><span data-stu-id="fece8-142">String</span></span>|<span data-ttu-id="fece8-143">Nome do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="fece8-143">Name of the award or honor.</span></span> |
|<span data-ttu-id="fece8-144">fracassa</span><span class="sxs-lookup"><span data-stu-id="fece8-144">inference</span></span>|[<span data-ttu-id="fece8-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="fece8-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="fece8-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="fece8-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="fece8-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fece8-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fece8-148">issuedDate</span><span class="sxs-lookup"><span data-stu-id="fece8-148">issuedDate</span></span>|<span data-ttu-id="fece8-149">Data</span><span class="sxs-lookup"><span data-stu-id="fece8-149">Date</span></span>|<span data-ttu-id="fece8-150">A data em que o prêmio ou honra foi concedido.</span><span class="sxs-lookup"><span data-stu-id="fece8-150">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="fece8-151">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="fece8-151">issuingAuthority</span></span>|<span data-ttu-id="fece8-152">String</span><span class="sxs-lookup"><span data-stu-id="fece8-152">String</span></span>|<span data-ttu-id="fece8-153">Autoridade que concedeu o prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="fece8-153">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="fece8-154">source</span><span class="sxs-lookup"><span data-stu-id="fece8-154">source</span></span>|[<span data-ttu-id="fece8-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="fece8-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="fece8-156">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="fece8-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="fece8-157">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fece8-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fece8-158">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="fece8-158">thumbnailUrl</span></span>|<span data-ttu-id="fece8-159">String</span><span class="sxs-lookup"><span data-stu-id="fece8-159">String</span></span>|<span data-ttu-id="fece8-160">URL que faz referência a uma miniatura do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="fece8-160">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="fece8-161">webUrl</span><span class="sxs-lookup"><span data-stu-id="fece8-161">webUrl</span></span>|<span data-ttu-id="fece8-162">String</span><span class="sxs-lookup"><span data-stu-id="fece8-162">String</span></span>|<span data-ttu-id="fece8-163">URL que faz referência ao prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="fece8-163">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="fece8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="fece8-164">Response</span></span>

<span data-ttu-id="fece8-165">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personAward](../resources/personaward.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fece8-165">If successful, this method returns a `201 Created` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fece8-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fece8-166">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="fece8-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="fece8-167">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fece8-168">C#</span><span class="sxs-lookup"><span data-stu-id="fece8-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personaward-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fece8-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fece8-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personaward-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fece8-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fece8-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personaward-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fece8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fece8-171">Response</span></span>
<span data-ttu-id="fece8-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fece8-172">**Note:** The response object shown here might be shortened for readability.</span></span>
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


