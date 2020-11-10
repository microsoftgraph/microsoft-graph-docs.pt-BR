---
title: Criar email
description: Criar um novo email.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da1d19a99182e7b242e162ae67b933db74cd995
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969671"
---
# <a name="create-itememail"></a><span data-ttu-id="56541-103">Criar email</span><span class="sxs-lookup"><span data-stu-id="56541-103">Create itemEmail</span></span>

<span data-ttu-id="56541-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56541-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56541-105">Criar um novo objeto de [email](../resources/itememail.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="56541-105">Create a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="56541-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="56541-106">Permissions</span></span>

<span data-ttu-id="56541-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56541-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56541-109">Permission type</span></span>                        | <span data-ttu-id="56541-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56541-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="56541-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56541-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="56541-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="56541-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="56541-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56541-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56541-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="56541-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="56541-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56541-115">Application</span></span>                            | <span data-ttu-id="56541-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56541-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="56541-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56541-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/emails
POST /users/{id | userPrincipalName}/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="56541-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56541-118">Request headers</span></span>
|<span data-ttu-id="56541-119">Nome</span><span class="sxs-lookup"><span data-stu-id="56541-119">Name</span></span>|<span data-ttu-id="56541-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="56541-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56541-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="56541-121">Authorization</span></span>|<span data-ttu-id="56541-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56541-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56541-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56541-124">Content-Type</span></span>|<span data-ttu-id="56541-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56541-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56541-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56541-127">Request body</span></span>
<span data-ttu-id="56541-128">No corpo da solicitação, forneça uma representação JSON do objeto de [email](../resources/itememail.md) .</span><span class="sxs-lookup"><span data-stu-id="56541-128">In the request body, supply a JSON representation of the [itemEmail](../resources/itememail.md) object.</span></span>

<span data-ttu-id="56541-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto item de [email](../resources/itememail.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="56541-129">The following table shows the properties that are possible to set when creating a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="56541-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56541-130">Property</span></span>|<span data-ttu-id="56541-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56541-131">Type</span></span>|<span data-ttu-id="56541-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56541-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56541-133">address</span><span class="sxs-lookup"><span data-stu-id="56541-133">address</span></span>|<span data-ttu-id="56541-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56541-134">String</span></span>|<span data-ttu-id="56541-135">O próprio endereço de email.</span><span class="sxs-lookup"><span data-stu-id="56541-135">The email address itself.</span></span>|
|<span data-ttu-id="56541-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="56541-136">allowedAudiences</span></span>|<span data-ttu-id="56541-137">String</span><span class="sxs-lookup"><span data-stu-id="56541-137">String</span></span>|<span data-ttu-id="56541-138">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="56541-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="56541-139">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="56541-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="56541-140">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="56541-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="56541-141">displayName</span><span class="sxs-lookup"><span data-stu-id="56541-141">displayName</span></span>|<span data-ttu-id="56541-142">String</span><span class="sxs-lookup"><span data-stu-id="56541-142">String</span></span>|<span data-ttu-id="56541-143">O nome ou rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="56541-143">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="56541-144">fracassa</span><span class="sxs-lookup"><span data-stu-id="56541-144">inference</span></span>|[<span data-ttu-id="56541-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="56541-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="56541-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="56541-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="56541-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="56541-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="56541-148">source</span><span class="sxs-lookup"><span data-stu-id="56541-148">source</span></span>|[<span data-ttu-id="56541-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="56541-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="56541-150">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="56541-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="56541-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="56541-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="56541-152">tipo</span><span class="sxs-lookup"><span data-stu-id="56541-152">type</span></span>|<span data-ttu-id="56541-153">emailtype</span><span class="sxs-lookup"><span data-stu-id="56541-153">emailType</span></span>|<span data-ttu-id="56541-154">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="56541-154">The type of email address.</span></span> <span data-ttu-id="56541-155">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="56541-155">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|



## <a name="response"></a><span data-ttu-id="56541-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="56541-156">Response</span></span>

<span data-ttu-id="56541-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto de [email](../resources/itememail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56541-157">If successful, this method returns a `201 Created` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56541-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56541-158">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="56541-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="56541-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/emails
Content-Type: application/json
Content-length: 383

{
  "address": "Innocenty.Popov@adventureworks.com",
}
```
# <a name="c"></a>[<span data-ttu-id="56541-160">C#</span><span class="sxs-lookup"><span data-stu-id="56541-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itememail-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56541-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56541-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itememail-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56541-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56541-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itememail-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56541-163">Java</span><span class="sxs-lookup"><span data-stu-id="56541-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itememail-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="56541-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="56541-164">Response</span></span>
<span data-ttu-id="56541-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56541-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": null,
  "type": null
}
```


