---
title: Criar endereços
description: Criar um novo objeto addresses.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a7338e553b483d4833c93036bf580aea4c9e4b00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812857"
---
# <a name="create-addresses"></a><span data-ttu-id="28059-103">Criar endereços</span><span class="sxs-lookup"><span data-stu-id="28059-103">Create addresses</span></span>
<span data-ttu-id="28059-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28059-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28059-105">Criar um novo objeto [myAddress](../resources/itemaddress.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="28059-105">Create a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28059-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28059-106">Permissions</span></span>

<span data-ttu-id="28059-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28059-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28059-109">Permission type</span></span>                        | <span data-ttu-id="28059-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28059-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="28059-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28059-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28059-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="28059-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="28059-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28059-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28059-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="28059-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="28059-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28059-115">Application</span></span>                            | <span data-ttu-id="28059-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28059-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="28059-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28059-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/addresses
POST /users/{id | userPrincipalName}/profile/addresses
```

## <a name="request-headers"></a><span data-ttu-id="28059-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28059-118">Request headers</span></span>
|<span data-ttu-id="28059-119">Nome</span><span class="sxs-lookup"><span data-stu-id="28059-119">Name</span></span>|<span data-ttu-id="28059-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="28059-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="28059-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="28059-121">Authorization</span></span>|<span data-ttu-id="28059-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28059-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="28059-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28059-124">Content-Type</span></span>|<span data-ttu-id="28059-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28059-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28059-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28059-127">Request body</span></span>
<span data-ttu-id="28059-128">No corpo da solicitação, forneça uma representação JSON do objeto [myAddress](../resources/itemaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="28059-128">In the request body, supply a JSON representation of the [itemAddress](../resources/itemaddress.md) object.</span></span>

<span data-ttu-id="28059-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto item de [endereço](../resources/itemaddress.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="28059-129">The following table shows the properties that are possible to set when creating a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="28059-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28059-130">Property</span></span>|<span data-ttu-id="28059-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="28059-131">Type</span></span>|<span data-ttu-id="28059-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="28059-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28059-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="28059-133">allowedAudiences</span></span>|<span data-ttu-id="28059-134">String</span><span class="sxs-lookup"><span data-stu-id="28059-134">String</span></span>|<span data-ttu-id="28059-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="28059-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="28059-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="28059-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="28059-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28059-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="28059-138">detalhada</span><span class="sxs-lookup"><span data-stu-id="28059-138">detail</span></span>|[<span data-ttu-id="28059-139">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="28059-139">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="28059-140">Detalhes sobre o próprio endereço.</span><span class="sxs-lookup"><span data-stu-id="28059-140">Details about the address itself.</span></span>|
|<span data-ttu-id="28059-141">displayName</span><span class="sxs-lookup"><span data-stu-id="28059-141">displayName</span></span>|<span data-ttu-id="28059-142">String</span><span class="sxs-lookup"><span data-stu-id="28059-142">String</span></span>|<span data-ttu-id="28059-143">Nome amigável que o usuário atribuiu a este endereço.</span><span class="sxs-lookup"><span data-stu-id="28059-143">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="28059-144">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="28059-144">geoCoordinates</span></span>|[<span data-ttu-id="28059-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="28059-145">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="28059-146">As geocoordenas do endereço.</span><span class="sxs-lookup"><span data-stu-id="28059-146">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="28059-147">fracassa</span><span class="sxs-lookup"><span data-stu-id="28059-147">inference</span></span>|[<span data-ttu-id="28059-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="28059-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="28059-149">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="28059-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="28059-150">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="28059-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="28059-151">source</span><span class="sxs-lookup"><span data-stu-id="28059-151">source</span></span>|[<span data-ttu-id="28059-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="28059-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="28059-153">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="28059-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="28059-154">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="28059-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
## <a name="response"></a><span data-ttu-id="28059-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="28059-155">Response</span></span>

<span data-ttu-id="28059-156">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [myAddress](../resources/itemaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28059-156">If successful, this method returns a `201 Created` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28059-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28059-157">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="28059-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="28059-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemaddress_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/addresses
Content-Type: application/json
Content-length: 497

{
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="28059-159">C#</span><span class="sxs-lookup"><span data-stu-id="28059-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28059-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28059-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28059-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28059-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="28059-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="28059-162">Response</span></span>
<span data-ttu-id="28059-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28059-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
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
  "displayName": "Home",
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
