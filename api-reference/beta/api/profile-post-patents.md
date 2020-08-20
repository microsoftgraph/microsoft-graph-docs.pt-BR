---
title: Criar patentes
description: Criar um novo objeto patenteados.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8345de1ca41dfd5e338b77c667ef06ae4b3bf31c
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820281"
---
# <a name="create-itempatent"></a><span data-ttu-id="23a21-103">Criar ispatente</span><span class="sxs-lookup"><span data-stu-id="23a21-103">Create itemPatent</span></span>

<span data-ttu-id="23a21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23a21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23a21-105">Criar um novo objeto de [patente](../resources/itempatent.md) dentro de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="23a21-105">Create a new [itemPatent](../resources/itempatent.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23a21-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23a21-106">Permissions</span></span>

<span data-ttu-id="23a21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23a21-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23a21-109">Permission type</span></span>                        | <span data-ttu-id="23a21-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23a21-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="23a21-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23a21-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23a21-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="23a21-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="23a21-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23a21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23a21-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="23a21-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="23a21-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23a21-115">Application</span></span>                            | <span data-ttu-id="23a21-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a21-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="23a21-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23a21-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/patents
POST /users/{id | userPrincipalName}/profile/patents
```

## <a name="request-headers"></a><span data-ttu-id="23a21-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23a21-118">Request headers</span></span>
|<span data-ttu-id="23a21-119">Nome</span><span class="sxs-lookup"><span data-stu-id="23a21-119">Name</span></span>|<span data-ttu-id="23a21-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="23a21-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23a21-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="23a21-121">Authorization</span></span>|<span data-ttu-id="23a21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23a21-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="23a21-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23a21-124">Content-Type</span></span>|<span data-ttu-id="23a21-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23a21-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23a21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23a21-127">Request body</span></span>
<span data-ttu-id="23a21-128">No corpo da solicitação, forneça uma representação JSON do objeto [ispatente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="23a21-128">In the request body, supply a JSON representation of the [itemPatent](../resources/itempatent.md) object.</span></span>

<span data-ttu-id="23a21-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto de item de [patente](../resources/itempatent.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="23a21-129">The following table shows the properties that are possible to set when creating a new [itemPatent](../resources/itempatent.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="23a21-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23a21-130">Property</span></span>|<span data-ttu-id="23a21-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="23a21-131">Type</span></span>|<span data-ttu-id="23a21-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="23a21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a21-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="23a21-133">allowedAudiences</span></span>|<span data-ttu-id="23a21-134">String</span><span class="sxs-lookup"><span data-stu-id="23a21-134">String</span></span>|<span data-ttu-id="23a21-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="23a21-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="23a21-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="23a21-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="23a21-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="23a21-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="23a21-138">description</span><span class="sxs-lookup"><span data-stu-id="23a21-138">description</span></span>|<span data-ttu-id="23a21-139">String</span><span class="sxs-lookup"><span data-stu-id="23a21-139">String</span></span>|<span data-ttu-id="23a21-140">Descpription da patente ou do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="23a21-140">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="23a21-141">displayName</span><span class="sxs-lookup"><span data-stu-id="23a21-141">displayName</span></span>|<span data-ttu-id="23a21-142">String</span><span class="sxs-lookup"><span data-stu-id="23a21-142">String</span></span>|<span data-ttu-id="23a21-143">Título da patente ou do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="23a21-143">Title of the patent or filing.</span></span> |
|<span data-ttu-id="23a21-144">fracassa</span><span class="sxs-lookup"><span data-stu-id="23a21-144">inference</span></span>|[<span data-ttu-id="23a21-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="23a21-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="23a21-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="23a21-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="23a21-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="23a21-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="23a21-148">ispending</span><span class="sxs-lookup"><span data-stu-id="23a21-148">isPending</span></span>        |<span data-ttu-id="23a21-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="23a21-149">Boolean</span></span>     |<span data-ttu-id="23a21-150">Indica que a patente está pendente.</span><span class="sxs-lookup"><span data-stu-id="23a21-150">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="23a21-151">issuedDate</span><span class="sxs-lookup"><span data-stu-id="23a21-151">issuedDate</span></span>       |<span data-ttu-id="23a21-152">Data</span><span class="sxs-lookup"><span data-stu-id="23a21-152">Date</span></span>        |<span data-ttu-id="23a21-153">A data em que a patente foi concedida.</span><span class="sxs-lookup"><span data-stu-id="23a21-153">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="23a21-154">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="23a21-154">issuingAuthority</span></span> |<span data-ttu-id="23a21-155">String</span><span class="sxs-lookup"><span data-stu-id="23a21-155">String</span></span>      |<span data-ttu-id="23a21-156">Autoridade que concedeu a patente.</span><span class="sxs-lookup"><span data-stu-id="23a21-156">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="23a21-157">number</span><span class="sxs-lookup"><span data-stu-id="23a21-157">number</span></span>           |<span data-ttu-id="23a21-158">String</span><span class="sxs-lookup"><span data-stu-id="23a21-158">String</span></span>      |<span data-ttu-id="23a21-159">O número de patente.</span><span class="sxs-lookup"><span data-stu-id="23a21-159">The patent number.</span></span>                      |
|<span data-ttu-id="23a21-160">source</span><span class="sxs-lookup"><span data-stu-id="23a21-160">source</span></span>|[<span data-ttu-id="23a21-161">personDataSource</span><span class="sxs-lookup"><span data-stu-id="23a21-161">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="23a21-162">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="23a21-162">Where the values originated if synced from another service.</span></span> <span data-ttu-id="23a21-163">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="23a21-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="23a21-164">webUrl</span><span class="sxs-lookup"><span data-stu-id="23a21-164">webUrl</span></span>           |<span data-ttu-id="23a21-165">String</span><span class="sxs-lookup"><span data-stu-id="23a21-165">String</span></span>      |<span data-ttu-id="23a21-166">URL que faz referência à patente ou ao arquivamento.</span><span class="sxs-lookup"><span data-stu-id="23a21-166">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="23a21-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="23a21-167">Response</span></span>

<span data-ttu-id="23a21-168">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [ispatente](../resources/itempatent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23a21-168">If successful, this method returns a `201 Created` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23a21-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23a21-169">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="23a21-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="23a21-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itempatent_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/patents
Content-Type: application/json
Content-length: 497

{
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="23a21-171">C#</span><span class="sxs-lookup"><span data-stu-id="23a21-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempatent-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23a21-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23a21-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempatent-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23a21-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23a21-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempatent-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="23a21-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="23a21-174">Response</span></span>
<span data-ttu-id="23a21-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23a21-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 201 Created
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
