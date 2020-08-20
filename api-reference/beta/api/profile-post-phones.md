---
title: Criar um número de telefone
description: Use esta API para criar um novo Multiphone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fcdb1c076d0fff4a3ae5bb6b49fdc77f6acb0aae
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819790"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="a52a6-103">Criar itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a52a6-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="a52a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a52a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a52a6-105">Use esta API para criar um novo objeto [MyPhone](../resources/itemphone.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a52a6-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a52a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a52a6-106">Permissions</span></span>

<span data-ttu-id="a52a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a52a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a52a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a52a6-109">Permission type</span></span>                        | <span data-ttu-id="a52a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a52a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a52a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a52a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a52a6-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a52a6-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a52a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a52a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a52a6-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a52a6-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a52a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a52a6-115">Application</span></span>                            | <span data-ttu-id="a52a6-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a52a6-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a52a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a52a6-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/phones
POST /users/{userId}/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="a52a6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a52a6-118">Request headers</span></span>
|<span data-ttu-id="a52a6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a52a6-119">Name</span></span>|<span data-ttu-id="a52a6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a52a6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a52a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a52a6-121">Authorization</span></span>|<span data-ttu-id="a52a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a52a6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a52a6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a52a6-124">Content-Type</span></span>|<span data-ttu-id="a52a6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a52a6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a52a6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a52a6-127">Request body</span></span>
<span data-ttu-id="a52a6-128">No corpo da solicitação, forneça uma representação JSON do objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="a52a6-128">In the request body, supply a JSON representation of the [itemPhone](../resources/itemphone.md) object.</span></span>

<span data-ttu-id="a52a6-129">A tabela a seguir mostra as propriedades que são possíveis de definir quando você cria um novo objeto [MyPhone](../resources/itemphone.md) em um perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="a52a6-129">The following table shows the properties that are possible to set when you create a new [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="a52a6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a52a6-130">Property</span></span>|<span data-ttu-id="a52a6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a52a6-131">Type</span></span>|<span data-ttu-id="a52a6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a52a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a52a6-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a52a6-133">allowedAudiences</span></span>|<span data-ttu-id="a52a6-134">String</span><span class="sxs-lookup"><span data-stu-id="a52a6-134">String</span></span>|<span data-ttu-id="a52a6-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="a52a6-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a52a6-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a52a6-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a52a6-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a52a6-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a52a6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a52a6-138">displayName</span></span>|<span data-ttu-id="a52a6-139">String</span><span class="sxs-lookup"><span data-stu-id="a52a6-139">String</span></span>|<span data-ttu-id="a52a6-140">Nome amigável o usuário atribuiu este número de telefone.</span><span class="sxs-lookup"><span data-stu-id="a52a6-140">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="a52a6-141">fracassa</span><span class="sxs-lookup"><span data-stu-id="a52a6-141">inference</span></span>|[<span data-ttu-id="a52a6-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a52a6-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a52a6-143">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="a52a6-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a52a6-144">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a52a6-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a52a6-145">number</span><span class="sxs-lookup"><span data-stu-id="a52a6-145">number</span></span>|<span data-ttu-id="a52a6-146">String</span><span class="sxs-lookup"><span data-stu-id="a52a6-146">String</span></span>|<span data-ttu-id="a52a6-147">Número de telefone fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="a52a6-147">Phone number provided by the user.</span></span>|
|<span data-ttu-id="a52a6-148">source</span><span class="sxs-lookup"><span data-stu-id="a52a6-148">source</span></span>|[<span data-ttu-id="a52a6-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="a52a6-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="a52a6-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="a52a6-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="a52a6-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a52a6-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a52a6-152">type</span><span class="sxs-lookup"><span data-stu-id="a52a6-152">type</span></span>|<span data-ttu-id="a52a6-153">PhoneType</span><span class="sxs-lookup"><span data-stu-id="a52a6-153">phoneType</span></span>|<span data-ttu-id="a52a6-154">O tipo de número de telefone dentro do objeto.</span><span class="sxs-lookup"><span data-stu-id="a52a6-154">The type of phone number within the object.</span></span> <span data-ttu-id="a52a6-155">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="a52a6-155">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="a52a6-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a52a6-156">Response</span></span>

<span data-ttu-id="a52a6-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [MyPhone](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a52a6-157">If successful, this method returns a `201 Created` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a52a6-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a52a6-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a52a6-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a52a6-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a52a6-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a52a6-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemphone_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/phones
Content-Type: application/json
Content-length: 382

{
  "displayName": "Car Phone",
  "number": "+7 499 342 22 13"
}
```
# <a name="c"></a>[<span data-ttu-id="a52a6-161">C#</span><span class="sxs-lookup"><span data-stu-id="a52a6-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a52a6-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a52a6-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a52a6-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a52a6-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a52a6-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="a52a6-164">Response</span></span>
<span data-ttu-id="a52a6-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a52a6-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
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
  "displayName": "Car Phone",
  "type": null,
  "number": "+7 499 342 22 13"
}
```
