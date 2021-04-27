---
title: Criar personInterest
description: Crie uma nova personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: e4f5648901ff1ed904d5e02fa278b6b9be329de8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036923"
---
# <a name="create-personinterest"></a><span data-ttu-id="122ad-103">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="122ad-103">Create personInterest</span></span>

<span data-ttu-id="122ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="122ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="122ad-105">Crie um novo [personInterest](.. /resources/personinterest.md] no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="122ad-105">Create a new [personInterest](../resources/personinterest.md] in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="122ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="122ad-106">Permissions</span></span>

<span data-ttu-id="122ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="122ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="122ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="122ad-109">Permission type</span></span>                        | <span data-ttu-id="122ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="122ad-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="122ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="122ad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="122ad-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="122ad-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="122ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="122ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="122ad-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="122ad-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="122ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="122ad-115">Application</span></span>                            | <span data-ttu-id="122ad-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="122ad-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="122ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="122ad-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="122ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="122ad-118">Request headers</span></span>

| <span data-ttu-id="122ad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="122ad-119">Name</span></span>      |<span data-ttu-id="122ad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="122ad-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="122ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="122ad-121">Authorization</span></span>  | <span data-ttu-id="122ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="122ad-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="122ad-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="122ad-124">Content-Type</span></span>   | <span data-ttu-id="122ad-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="122ad-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="122ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="122ad-127">Request body</span></span>

<span data-ttu-id="122ad-128">No corpo da solicitação, fornece uma representação JSON do [objeto personInterest.](../resources/personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="122ad-128">In the request body, supply a JSON representation of the [personInterest](../resources/personinterest.md) object.</span></span>

<span data-ttu-id="122ad-129">A tabela a seguir mostra as propriedades que são possíveis de definir dentro de um novo [objeto personInterest](../resources/personinterest.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="122ad-129">The following table shows the properties that are possible to set within a new [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="122ad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="122ad-130">Property</span></span>|<span data-ttu-id="122ad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="122ad-131">Type</span></span>|<span data-ttu-id="122ad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="122ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="122ad-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="122ad-133">allowedAudiences</span></span>|<span data-ttu-id="122ad-134">String</span><span class="sxs-lookup"><span data-stu-id="122ad-134">String</span></span>|<span data-ttu-id="122ad-135">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="122ad-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="122ad-136">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="122ad-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="122ad-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="122ad-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="122ad-138">categories</span><span class="sxs-lookup"><span data-stu-id="122ad-138">categories</span></span>|<span data-ttu-id="122ad-139">String collection</span><span class="sxs-lookup"><span data-stu-id="122ad-139">String collection</span></span>|<span data-ttu-id="122ad-140">Contém categorias que um usuário associou ao interesse (por exemplo, recipies pessoais).</span><span class="sxs-lookup"><span data-stu-id="122ad-140">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="122ad-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="122ad-141">collaborationTags</span></span>|<span data-ttu-id="122ad-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="122ad-142">String collection</span></span>|<span data-ttu-id="122ad-143">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="122ad-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="122ad-144">Os valores permitidos na coleção são: `askMeAbout` `ableToMentor` , , , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="122ad-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="122ad-145">description</span><span class="sxs-lookup"><span data-stu-id="122ad-145">description</span></span>|<span data-ttu-id="122ad-146">String</span><span class="sxs-lookup"><span data-stu-id="122ad-146">String</span></span>|<span data-ttu-id="122ad-147">Contém uma descrição do interesse.</span><span class="sxs-lookup"><span data-stu-id="122ad-147">Contains a description of the interest.</span></span>|
|<span data-ttu-id="122ad-148">displayName</span><span class="sxs-lookup"><span data-stu-id="122ad-148">displayName</span></span>|<span data-ttu-id="122ad-149">String</span><span class="sxs-lookup"><span data-stu-id="122ad-149">String</span></span>|<span data-ttu-id="122ad-150">Contém um nome amigável para o interesse.</span><span class="sxs-lookup"><span data-stu-id="122ad-150">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="122ad-151">inferência</span><span class="sxs-lookup"><span data-stu-id="122ad-151">inference</span></span>|[<span data-ttu-id="122ad-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="122ad-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="122ad-153">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="122ad-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="122ad-154">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="122ad-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="122ad-155">source</span><span class="sxs-lookup"><span data-stu-id="122ad-155">source</span></span>|[<span data-ttu-id="122ad-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="122ad-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="122ad-157">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="122ad-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="122ad-158">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="122ad-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="122ad-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="122ad-159">webUrl</span></span>|<span data-ttu-id="122ad-160">String</span><span class="sxs-lookup"><span data-stu-id="122ad-160">String</span></span>|<span data-ttu-id="122ad-161">Contém um link para uma página da Web ou recurso sobre o interesse.</span><span class="sxs-lookup"><span data-stu-id="122ad-161">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="122ad-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="122ad-162">Response</span></span>

<span data-ttu-id="122ad-163">Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo objeto [personInterest](../resources/personinterest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="122ad-163">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="122ad-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="122ad-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="122ad-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="122ad-165">Request</span></span>

<span data-ttu-id="122ad-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="122ad-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="122ad-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="122ad-167">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="122ad-168">C#</span><span class="sxs-lookup"><span data-stu-id="122ad-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="122ad-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="122ad-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="122ad-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="122ad-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="122ad-171">Java</span><span class="sxs-lookup"><span data-stu-id="122ad-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personinterest-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="122ad-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="122ad-172">Response</span></span>

<span data-ttu-id="122ad-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="122ad-173">The following is an example of the response.</span></span>

> <span data-ttu-id="122ad-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="122ad-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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


