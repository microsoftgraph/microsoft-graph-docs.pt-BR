---
title: Criar personWebsite
description: Crie um novo personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f05a1cab47ef5500242cbda9fd0452a4e78a4750
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036699"
---
# <a name="create-personwebsite"></a><span data-ttu-id="fb7f1-103">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="fb7f1-103">Create personWebsite</span></span>

<span data-ttu-id="fb7f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb7f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb7f1-105">Crie um novo [objeto personWebsite](../resources/personwebsite.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="fb7f1-105">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb7f1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb7f1-106">Permissions</span></span>

<span data-ttu-id="fb7f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb7f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb7f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb7f1-109">Permission type</span></span>                        | <span data-ttu-id="fb7f1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb7f1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fb7f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb7f1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb7f1-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7f1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fb7f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb7f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb7f1-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7f1-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fb7f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb7f1-115">Application</span></span>                            | <span data-ttu-id="fb7f1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7f1-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="fb7f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb7f1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
POST /users/{id | userPrincipalName}/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="fb7f1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7f1-118">Request headers</span></span>

| <span data-ttu-id="fb7f1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fb7f1-119">Name</span></span>           | <span data-ttu-id="fb7f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7f1-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="fb7f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb7f1-121">Authorization</span></span>  | <span data-ttu-id="fb7f1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="fb7f1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb7f1-124">Content-Type</span></span>   | <span data-ttu-id="fb7f1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb7f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7f1-127">Request body</span></span>

<span data-ttu-id="fb7f1-128">No corpo da solicitação, fornece uma representação JSON do [objeto personWebsite.](../resources/personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="fb7f1-128">In the request body, supply a JSON representation of the [personWebsite](../resources/personwebsite.md) object.</span></span>

<span data-ttu-id="fb7f1-129">A tabela a seguir mostra as propriedades que são possíveis de definir dentro de um novo [objeto personWebsite](../resources/personwebsite.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="fb7f1-129">The following table shows the properties that are possible to set within a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="fb7f1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb7f1-130">Property</span></span>|<span data-ttu-id="fb7f1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb7f1-131">Type</span></span>|<span data-ttu-id="fb7f1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb7f1-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="fb7f1-133">allowedAudiences</span></span>|<span data-ttu-id="fb7f1-134">String</span><span class="sxs-lookup"><span data-stu-id="fb7f1-134">String</span></span>|<span data-ttu-id="fb7f1-135">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="fb7f1-136">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fb7f1-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="fb7f1-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fb7f1-138">categories</span><span class="sxs-lookup"><span data-stu-id="fb7f1-138">categories</span></span>|<span data-ttu-id="fb7f1-139">String collection</span><span class="sxs-lookup"><span data-stu-id="fb7f1-139">String collection</span></span>|<span data-ttu-id="fb7f1-140">Contém categorias que um usuário associou ao site (por exemplo, receitas pessoais).</span><span class="sxs-lookup"><span data-stu-id="fb7f1-140">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="fb7f1-141">description</span><span class="sxs-lookup"><span data-stu-id="fb7f1-141">description</span></span>|<span data-ttu-id="fb7f1-142">String</span><span class="sxs-lookup"><span data-stu-id="fb7f1-142">String</span></span>|<span data-ttu-id="fb7f1-143">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-143">Contains a description of the website.</span></span>|
|<span data-ttu-id="fb7f1-144">displayName</span><span class="sxs-lookup"><span data-stu-id="fb7f1-144">displayName</span></span>|<span data-ttu-id="fb7f1-145">String</span><span class="sxs-lookup"><span data-stu-id="fb7f1-145">String</span></span>|<span data-ttu-id="fb7f1-146">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-146">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="fb7f1-147">inferência</span><span class="sxs-lookup"><span data-stu-id="fb7f1-147">inference</span></span>|[<span data-ttu-id="fb7f1-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="fb7f1-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="fb7f1-149">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="fb7f1-150">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fb7f1-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fb7f1-151">source</span><span class="sxs-lookup"><span data-stu-id="fb7f1-151">source</span></span>|[<span data-ttu-id="fb7f1-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="fb7f1-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="fb7f1-153">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="fb7f1-154">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fb7f1-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fb7f1-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="fb7f1-155">webUrl</span></span>|<span data-ttu-id="fb7f1-156">String</span><span class="sxs-lookup"><span data-stu-id="fb7f1-156">String</span></span>|<span data-ttu-id="fb7f1-157">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-157">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="fb7f1-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb7f1-158">Response</span></span>

<span data-ttu-id="fb7f1-159">Se tiver êxito, este método retornará `201, Created` o código de resposta e um novo objeto [personWebsite](../resources/personwebsite.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-159">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb7f1-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb7f1-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb7f1-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7f1-161">Request</span></span>

<span data-ttu-id="fb7f1-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb7f1-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb7f1-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
Content-type: application/json

{
  "categories": [
    "football"
  ],
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```
# <a name="c"></a>[<span data-ttu-id="fb7f1-164">C#</span><span class="sxs-lookup"><span data-stu-id="fb7f1-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personwebsite-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb7f1-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb7f1-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personwebsite-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb7f1-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb7f1-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personwebsite-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb7f1-167">Java</span><span class="sxs-lookup"><span data-stu-id="fb7f1-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personwebsite-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb7f1-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb7f1-168">Response</span></span>

<span data-ttu-id="fb7f1-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-169">The following is an example of the response.</span></span>

> <span data-ttu-id="fb7f1-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb7f1-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "categories": [
    "football"
  ],
  "description": null,
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```


