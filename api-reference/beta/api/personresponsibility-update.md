---
title: Atualizar personResponsibility
description: Atualiza as propriedades de um objeto personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9c4696ae3c9f97a6f256c65844b062e0f7882c3e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812877"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="791a5-103">Atualizar personResponsibility</span><span class="sxs-lookup"><span data-stu-id="791a5-103">Update personResponsibility</span></span>
<span data-ttu-id="791a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="791a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="791a5-105">Atualiza as propriedades de um objeto [personResponsibility](../resources/personresponsibility.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="791a5-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="791a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="791a5-106">Permissions</span></span>

<span data-ttu-id="791a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="791a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="791a5-109">Permission type</span></span>                        | <span data-ttu-id="791a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="791a5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="791a5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="791a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="791a5-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="791a5-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="791a5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="791a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791a5-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="791a5-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="791a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="791a5-115">Application</span></span>                            | <span data-ttu-id="791a5-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="791a5-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="791a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="791a5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="791a5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="791a5-118">Request headers</span></span>
|<span data-ttu-id="791a5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="791a5-119">Name</span></span>|<span data-ttu-id="791a5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="791a5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="791a5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="791a5-121">Authorization</span></span>|<span data-ttu-id="791a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="791a5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="791a5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="791a5-124">Content-Type</span></span>|<span data-ttu-id="791a5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="791a5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="791a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="791a5-127">Request body</span></span>
<span data-ttu-id="791a5-128">No corpo da solicitação, forneça uma representação JSON do objeto [personResponsibility](../resources/personresponsibility.md) .</span><span class="sxs-lookup"><span data-stu-id="791a5-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="791a5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [personResponsibility](../resources/personresponsibility.md).</span><span class="sxs-lookup"><span data-stu-id="791a5-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="791a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="791a5-130">Property</span></span>|<span data-ttu-id="791a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="791a5-131">Type</span></span>|<span data-ttu-id="791a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="791a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="791a5-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="791a5-133">allowedAudiences</span></span>|<span data-ttu-id="791a5-134">String</span><span class="sxs-lookup"><span data-stu-id="791a5-134">String</span></span>|<span data-ttu-id="791a5-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="791a5-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="791a5-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="791a5-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="791a5-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="791a5-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="791a5-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="791a5-138">collaborationTags</span></span>|<span data-ttu-id="791a5-139">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="791a5-139">String collection</span></span>|<span data-ttu-id="791a5-140">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="791a5-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="791a5-141">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="791a5-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="791a5-142">description</span><span class="sxs-lookup"><span data-stu-id="791a5-142">description</span></span>|<span data-ttu-id="791a5-143">String</span><span class="sxs-lookup"><span data-stu-id="791a5-143">String</span></span>|<span data-ttu-id="791a5-144">Descrição da responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="791a5-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="791a5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="791a5-145">displayName</span></span>|<span data-ttu-id="791a5-146">String</span><span class="sxs-lookup"><span data-stu-id="791a5-146">String</span></span>|<span data-ttu-id="791a5-147">Contém um nome amigável para a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="791a5-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="791a5-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="791a5-148">inference</span></span>|[<span data-ttu-id="791a5-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="791a5-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="791a5-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="791a5-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="791a5-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="791a5-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="791a5-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="791a5-152">webUrl</span></span>|<span data-ttu-id="791a5-153">String</span><span class="sxs-lookup"><span data-stu-id="791a5-153">String</span></span>|<span data-ttu-id="791a5-154">Contém um link para uma página da Web ou recurso sobre a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="791a5-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="791a5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="791a5-155">Response</span></span>

<span data-ttu-id="791a5-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personResponsibility](../resources/personresponsibility.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="791a5-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="791a5-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="791a5-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="791a5-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="791a5-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="791a5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="791a5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="791a5-160">C#</span><span class="sxs-lookup"><span data-stu-id="791a5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="791a5-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="791a5-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="791a5-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="791a5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="791a5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="791a5-163">Response</span></span>
<span data-ttu-id="791a5-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="791a5-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
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
  "source": null,
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
