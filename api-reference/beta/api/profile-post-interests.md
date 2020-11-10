---
title: Criar personInterest
description: Criar um novo personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: 156e9f6cef6c0b0f6e9def42fc4d2417706e426b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975369"
---
# <a name="create-personinterest"></a><span data-ttu-id="11a47-103">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="11a47-103">Create personInterest</span></span>

<span data-ttu-id="11a47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11a47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a47-105">Criar um novo [personInterest] (.. /Resources/personinterest.MD] no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="11a47-105">Create a new [personInterest](../resources/personinterest.md] in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="11a47-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11a47-106">Permissions</span></span>

<span data-ttu-id="11a47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11a47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11a47-109">Permission type</span></span>                        | <span data-ttu-id="11a47-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11a47-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11a47-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11a47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11a47-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11a47-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="11a47-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11a47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11a47-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11a47-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="11a47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11a47-115">Application</span></span>                            | <span data-ttu-id="11a47-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11a47-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="11a47-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11a47-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="11a47-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11a47-118">Request headers</span></span>

| <span data-ttu-id="11a47-119">Nome</span><span class="sxs-lookup"><span data-stu-id="11a47-119">Name</span></span>      |<span data-ttu-id="11a47-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11a47-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11a47-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11a47-121">Authorization</span></span>  | <span data-ttu-id="11a47-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11a47-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="11a47-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11a47-124">Content-Type</span></span>   | <span data-ttu-id="11a47-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11a47-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11a47-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11a47-127">Request body</span></span>

<span data-ttu-id="11a47-128">No corpo da solicitação, forneça uma representação JSON do objeto [personInterest](../resources/personinterest.md) .</span><span class="sxs-lookup"><span data-stu-id="11a47-128">In the request body, supply a JSON representation of the [personInterest](../resources/personinterest.md) object.</span></span>

<span data-ttu-id="11a47-129">A tabela a seguir mostra as propriedades que são possíveis de definir em um novo objeto [personInterest](../resources/personinterest.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="11a47-129">The following table shows the properties that are possible to set within a new [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="11a47-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11a47-130">Property</span></span>|<span data-ttu-id="11a47-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11a47-131">Type</span></span>|<span data-ttu-id="11a47-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11a47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11a47-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="11a47-133">allowedAudiences</span></span>|<span data-ttu-id="11a47-134">String</span><span class="sxs-lookup"><span data-stu-id="11a47-134">String</span></span>|<span data-ttu-id="11a47-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="11a47-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="11a47-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="11a47-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="11a47-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="11a47-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="11a47-138">categories</span><span class="sxs-lookup"><span data-stu-id="11a47-138">categories</span></span>|<span data-ttu-id="11a47-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11a47-139">String collection</span></span>|<span data-ttu-id="11a47-140">Contém categorias que um usuário associou aos juros (por exemplo, pessoal, recipies).</span><span class="sxs-lookup"><span data-stu-id="11a47-140">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="11a47-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="11a47-141">collaborationTags</span></span>|<span data-ttu-id="11a47-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11a47-142">String collection</span></span>|<span data-ttu-id="11a47-143">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="11a47-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="11a47-144">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="11a47-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="11a47-145">description</span><span class="sxs-lookup"><span data-stu-id="11a47-145">description</span></span>|<span data-ttu-id="11a47-146">String</span><span class="sxs-lookup"><span data-stu-id="11a47-146">String</span></span>|<span data-ttu-id="11a47-147">Contém uma descrição dos juros.</span><span class="sxs-lookup"><span data-stu-id="11a47-147">Contains a description of the interest.</span></span>|
|<span data-ttu-id="11a47-148">displayName</span><span class="sxs-lookup"><span data-stu-id="11a47-148">displayName</span></span>|<span data-ttu-id="11a47-149">String</span><span class="sxs-lookup"><span data-stu-id="11a47-149">String</span></span>|<span data-ttu-id="11a47-150">Contém um nome amigável para os juros.</span><span class="sxs-lookup"><span data-stu-id="11a47-150">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="11a47-151">fracassa</span><span class="sxs-lookup"><span data-stu-id="11a47-151">inference</span></span>|[<span data-ttu-id="11a47-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="11a47-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="11a47-153">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="11a47-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="11a47-154">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="11a47-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="11a47-155">source</span><span class="sxs-lookup"><span data-stu-id="11a47-155">source</span></span>|[<span data-ttu-id="11a47-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="11a47-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="11a47-157">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="11a47-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="11a47-158">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="11a47-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="11a47-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="11a47-159">webUrl</span></span>|<span data-ttu-id="11a47-160">String</span><span class="sxs-lookup"><span data-stu-id="11a47-160">String</span></span>|<span data-ttu-id="11a47-161">Contém um link para uma página da Web ou recurso sobre os juros.</span><span class="sxs-lookup"><span data-stu-id="11a47-161">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="11a47-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="11a47-162">Response</span></span>

<span data-ttu-id="11a47-163">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [personInterest](../resources/personinterest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11a47-163">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11a47-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11a47-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11a47-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11a47-165">Request</span></span>

<span data-ttu-id="11a47-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11a47-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11a47-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="11a47-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com"
}
```
# <a name="c"></a>[<span data-ttu-id="11a47-168">C#</span><span class="sxs-lookup"><span data-stu-id="11a47-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11a47-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11a47-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11a47-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11a47-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11a47-171">Java</span><span class="sxs-lookup"><span data-stu-id="11a47-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personinterest-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11a47-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="11a47-172">Response</span></span>

<span data-ttu-id="11a47-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11a47-173">The following is an example of the response.</span></span>

> <span data-ttu-id="11a47-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11a47-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


