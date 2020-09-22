---
title: Atualizar o número de telefone
description: Atualiza as propriedades de um objeto MyPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 823dbabbe2936cc7c75af4a480610c7c5d71085c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999346"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="8015d-103">Atualizar itemphonenumber</span><span class="sxs-lookup"><span data-stu-id="8015d-103">Update itemphonenumber</span></span>

<span data-ttu-id="8015d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8015d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8015d-105">Atualizar as propriedades de um objeto [MyPhone](../resources/itemphone.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8015d-105">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8015d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8015d-106">Permissions</span></span>

<span data-ttu-id="8015d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8015d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8015d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8015d-109">Permission type</span></span>                        | <span data-ttu-id="8015d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8015d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8015d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8015d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8015d-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8015d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8015d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8015d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8015d-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8015d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8015d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8015d-115">Application</span></span>                            | <span data-ttu-id="8015d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8015d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8015d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8015d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/phones/{id}
PATCH /user/{userId}/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8015d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8015d-118">Request headers</span></span>
|<span data-ttu-id="8015d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8015d-119">Name</span></span>|<span data-ttu-id="8015d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8015d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8015d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8015d-121">Authorization</span></span>|<span data-ttu-id="8015d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8015d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8015d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8015d-124">Content-Type</span></span>|<span data-ttu-id="8015d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8015d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8015d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8015d-127">Request body</span></span>

<span data-ttu-id="8015d-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8015d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8015d-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8015d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8015d-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8015d-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="8015d-131">A tabela a seguir mostra as propriedades que são possíveis de definir quando você atualiza um objeto [MyPhone](../resources/itemphone.md) em um perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="8015d-131">The following table shows the properties that are possible to set when you update an [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="8015d-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8015d-132">Property</span></span>|<span data-ttu-id="8015d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="8015d-133">Type</span></span>|<span data-ttu-id="8015d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8015d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8015d-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8015d-135">allowedAudiences</span></span>|<span data-ttu-id="8015d-136">String</span><span class="sxs-lookup"><span data-stu-id="8015d-136">String</span></span>|<span data-ttu-id="8015d-137">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="8015d-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8015d-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8015d-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8015d-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8015d-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8015d-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8015d-140">displayName</span></span>|<span data-ttu-id="8015d-141">String</span><span class="sxs-lookup"><span data-stu-id="8015d-141">String</span></span>|<span data-ttu-id="8015d-142">Nome amigável o usuário atribuiu este número de telefone.</span><span class="sxs-lookup"><span data-stu-id="8015d-142">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="8015d-143">fracassa</span><span class="sxs-lookup"><span data-stu-id="8015d-143">inference</span></span>|[<span data-ttu-id="8015d-144">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8015d-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8015d-145">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="8015d-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8015d-146">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8015d-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8015d-147">number</span><span class="sxs-lookup"><span data-stu-id="8015d-147">number</span></span>|<span data-ttu-id="8015d-148">String</span><span class="sxs-lookup"><span data-stu-id="8015d-148">String</span></span>|<span data-ttu-id="8015d-149">Número de telefone fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8015d-149">Phone number provided by the user.</span></span>|
|<span data-ttu-id="8015d-150">source</span><span class="sxs-lookup"><span data-stu-id="8015d-150">source</span></span>|[<span data-ttu-id="8015d-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8015d-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8015d-152">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="8015d-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8015d-153">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8015d-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8015d-154">tipo</span><span class="sxs-lookup"><span data-stu-id="8015d-154">type</span></span>|<span data-ttu-id="8015d-155">PhoneType</span><span class="sxs-lookup"><span data-stu-id="8015d-155">phoneType</span></span>|<span data-ttu-id="8015d-156">O tipo de número de telefone dentro do objeto.</span><span class="sxs-lookup"><span data-stu-id="8015d-156">The type of phone number within the object.</span></span> <span data-ttu-id="8015d-157">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="8015d-157">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="8015d-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="8015d-158">Response</span></span>

<span data-ttu-id="8015d-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [MyPhone](../resources/itemphone.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8015d-159">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8015d-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8015d-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8015d-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8015d-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="8015d-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8015d-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/phones/{id}
Content-Type: application/json
Content-length: 382

{
  "type": "other"
}
```
# <a name="c"></a>[<span data-ttu-id="8015d-163">C#</span><span class="sxs-lookup"><span data-stu-id="8015d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8015d-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8015d-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8015d-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8015d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8015d-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8015d-166">Response</span></span>
<span data-ttu-id="8015d-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8015d-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
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
  "displayName": "Car Phone",
  "type": "other",
  "number": "+7 499 342 22 13"
}
```


