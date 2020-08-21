---
title: Criar endereços
description: Criar um novo objeto addresses.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2dab94f8aefe12a073041ade6a6deedcee07f8ab
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820207"
---
# <a name="create-addresses"></a><span data-ttu-id="d021c-103">Criar endereços</span><span class="sxs-lookup"><span data-stu-id="d021c-103">Create addresses</span></span>
<span data-ttu-id="d021c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d021c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d021c-105">Criar um novo objeto [myAddress](../resources/itemaddress.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d021c-105">Create a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d021c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d021c-106">Permissions</span></span>

<span data-ttu-id="d021c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d021c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d021c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d021c-109">Permission type</span></span>                        | <span data-ttu-id="d021c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d021c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d021c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d021c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d021c-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d021c-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d021c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d021c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d021c-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d021c-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d021c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d021c-115">Application</span></span>                            | <span data-ttu-id="d021c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d021c-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="d021c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d021c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/addresses
POST /users/{id | userPrincipalName}/profile/addresses
```

## <a name="request-headers"></a><span data-ttu-id="d021c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d021c-118">Request headers</span></span>
|<span data-ttu-id="d021c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d021c-119">Name</span></span>|<span data-ttu-id="d021c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d021c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d021c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d021c-121">Authorization</span></span>|<span data-ttu-id="d021c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d021c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d021c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d021c-124">Content-Type</span></span>|<span data-ttu-id="d021c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d021c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d021c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d021c-127">Request body</span></span>
<span data-ttu-id="d021c-128">No corpo da solicitação, forneça uma representação JSON do objeto [myAddress](../resources/itemaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="d021c-128">In the request body, supply a JSON representation of the [itemAddress](../resources/itemaddress.md) object.</span></span>

<span data-ttu-id="d021c-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto item de [endereço](../resources/itemaddress.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d021c-129">The following table shows the properties that are possible to set when creating a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="d021c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d021c-130">Property</span></span>|<span data-ttu-id="d021c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d021c-131">Type</span></span>|<span data-ttu-id="d021c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d021c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d021c-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d021c-133">allowedAudiences</span></span>|<span data-ttu-id="d021c-134">String</span><span class="sxs-lookup"><span data-stu-id="d021c-134">String</span></span>|<span data-ttu-id="d021c-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="d021c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d021c-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d021c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d021c-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d021c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d021c-138">detalhada</span><span class="sxs-lookup"><span data-stu-id="d021c-138">detail</span></span>|[<span data-ttu-id="d021c-139">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d021c-139">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="d021c-140">Detalhes sobre o próprio endereço.</span><span class="sxs-lookup"><span data-stu-id="d021c-140">Details about the address itself.</span></span>|
|<span data-ttu-id="d021c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d021c-141">displayName</span></span>|<span data-ttu-id="d021c-142">String</span><span class="sxs-lookup"><span data-stu-id="d021c-142">String</span></span>|<span data-ttu-id="d021c-143">Nome amigável que o usuário atribuiu a este endereço.</span><span class="sxs-lookup"><span data-stu-id="d021c-143">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="d021c-144">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d021c-144">geoCoordinates</span></span>|[<span data-ttu-id="d021c-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d021c-145">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="d021c-146">As geocoordenas do endereço.</span><span class="sxs-lookup"><span data-stu-id="d021c-146">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="d021c-147">fracassa</span><span class="sxs-lookup"><span data-stu-id="d021c-147">inference</span></span>|[<span data-ttu-id="d021c-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d021c-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d021c-149">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="d021c-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d021c-150">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d021c-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d021c-151">source</span><span class="sxs-lookup"><span data-stu-id="d021c-151">source</span></span>|[<span data-ttu-id="d021c-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="d021c-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="d021c-153">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="d021c-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="d021c-154">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d021c-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
## <a name="response"></a><span data-ttu-id="d021c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d021c-155">Response</span></span>

<span data-ttu-id="d021c-156">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [myAddress](../resources/itemaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d021c-156">If successful, this method returns a `201 Created` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d021c-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d021c-157">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="d021c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="d021c-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d021c-159">C#</span><span class="sxs-lookup"><span data-stu-id="d021c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemaddress-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d021c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d021c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemaddress-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d021c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d021c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemaddress-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d021c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d021c-162">Response</span></span>
<span data-ttu-id="d021c-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d021c-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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