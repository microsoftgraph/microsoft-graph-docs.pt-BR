---
title: Criar responsabilidades
description: Criar um novo objeto responsabilidades.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9c0907217bd75b79bc7e200dfc5d9deb901a2bfe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034342"
---
# <a name="create-personresponsibility"></a><span data-ttu-id="f38b3-103">Criar personResponsibility</span><span class="sxs-lookup"><span data-stu-id="f38b3-103">Create personResponsibility</span></span>
<span data-ttu-id="f38b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f38b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f38b3-105">Criar um novo objeto [personResponsibility](../resources/personresponsibility.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f38b3-105">Create a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f38b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f38b3-106">Permissions</span></span>

<span data-ttu-id="f38b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f38b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f38b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f38b3-109">Permission type</span></span>                        | <span data-ttu-id="f38b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f38b3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f38b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f38b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f38b3-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f38b3-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f38b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f38b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f38b3-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f38b3-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f38b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f38b3-115">Application</span></span>                            | <span data-ttu-id="f38b3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f38b3-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f38b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f38b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/responsibilities
POST /users/{id | userPrincipalName}/profile/responsibilities
```

## <a name="request-headers"></a><span data-ttu-id="f38b3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f38b3-118">Request headers</span></span>
|<span data-ttu-id="f38b3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f38b3-119">Name</span></span>|<span data-ttu-id="f38b3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38b3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f38b3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f38b3-121">Authorization</span></span>|<span data-ttu-id="f38b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f38b3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f38b3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f38b3-124">Content-Type</span></span>|<span data-ttu-id="f38b3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f38b3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f38b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f38b3-127">Request body</span></span>
<span data-ttu-id="f38b3-128">No corpo da solicitação, forneça uma representação JSON do objeto [personResponsibility](../resources/personresponsibility.md) .</span><span class="sxs-lookup"><span data-stu-id="f38b3-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="f38b3-129">A tabela a seguir mostra as propriedades que são possíveis de definir em um novo objeto [personResponsibility](../resources/personresponsibility.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f38b3-129">The following table shows the properties that are possible to set within a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="f38b3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f38b3-130">Property</span></span>|<span data-ttu-id="f38b3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38b3-131">Type</span></span>|<span data-ttu-id="f38b3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f38b3-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="f38b3-133">allowedAudiences</span></span>|<span data-ttu-id="f38b3-134">String</span><span class="sxs-lookup"><span data-stu-id="f38b3-134">String</span></span>|<span data-ttu-id="f38b3-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="f38b3-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f38b3-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f38b3-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f38b3-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f38b3-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f38b3-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="f38b3-138">collaborationTags</span></span>|<span data-ttu-id="f38b3-139">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f38b3-139">String collection</span></span>|<span data-ttu-id="f38b3-140">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="f38b3-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="f38b3-141">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="f38b3-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="f38b3-142">description</span><span class="sxs-lookup"><span data-stu-id="f38b3-142">description</span></span>|<span data-ttu-id="f38b3-143">String</span><span class="sxs-lookup"><span data-stu-id="f38b3-143">String</span></span>|<span data-ttu-id="f38b3-144">Descrição da responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="f38b3-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="f38b3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f38b3-145">displayName</span></span>|<span data-ttu-id="f38b3-146">String</span><span class="sxs-lookup"><span data-stu-id="f38b3-146">String</span></span>|<span data-ttu-id="f38b3-147">Contém um nome amigável para a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="f38b3-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="f38b3-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="f38b3-148">inference</span></span>|[<span data-ttu-id="f38b3-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="f38b3-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f38b3-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="f38b3-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f38b3-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f38b3-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f38b3-152">source</span><span class="sxs-lookup"><span data-stu-id="f38b3-152">source</span></span>|[<span data-ttu-id="f38b3-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="f38b3-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="f38b3-154">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="f38b3-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="f38b3-155">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f38b3-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f38b3-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="f38b3-156">webUrl</span></span>|<span data-ttu-id="f38b3-157">String</span><span class="sxs-lookup"><span data-stu-id="f38b3-157">String</span></span>|<span data-ttu-id="f38b3-158">Contém um link para uma página da Web ou recurso sobre a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="f38b3-158">Contains a link to a web page or resource about the responsibility.</span></span>|

## <a name="response"></a><span data-ttu-id="f38b3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38b3-159">Response</span></span>

<span data-ttu-id="f38b3-160">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personResponsibility](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f38b3-160">If successful, this method returns a `201 Created` response code and a [personResponsibility](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f38b3-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f38b3-161">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="f38b3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f38b3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="f38b3-163">C#</span><span class="sxs-lookup"><span data-stu-id="f38b3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f38b3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f38b3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f38b3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f38b3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f38b3-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38b3-166">Response</span></span>
<span data-ttu-id="f38b3-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f38b3-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


