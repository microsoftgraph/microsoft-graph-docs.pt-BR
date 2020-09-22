---
title: Atualizar personResponsibility
description: Atualiza as propriedades de um objeto personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 38ca672825c49f0149dcf9b06b4c57d8df92c0e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017364"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="fc78c-103">Atualizar personResponsibility</span><span class="sxs-lookup"><span data-stu-id="fc78c-103">Update personResponsibility</span></span>
<span data-ttu-id="fc78c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc78c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc78c-105">Atualiza as propriedades de um objeto [personResponsibility](../resources/personresponsibility.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fc78c-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc78c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc78c-106">Permissions</span></span>

<span data-ttu-id="fc78c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc78c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc78c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc78c-109">Permission type</span></span>                        | <span data-ttu-id="fc78c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc78c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="fc78c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc78c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc78c-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fc78c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fc78c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc78c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc78c-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fc78c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fc78c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc78c-115">Application</span></span>                            | <span data-ttu-id="fc78c-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fc78c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="fc78c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc78c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fc78c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc78c-118">Request headers</span></span>
|<span data-ttu-id="fc78c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc78c-119">Name</span></span>|<span data-ttu-id="fc78c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc78c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fc78c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc78c-121">Authorization</span></span>|<span data-ttu-id="fc78c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc78c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fc78c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc78c-124">Content-Type</span></span>|<span data-ttu-id="fc78c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc78c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc78c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc78c-127">Request body</span></span>
<span data-ttu-id="fc78c-128">No corpo da solicitação, forneça uma representação JSON do objeto [personResponsibility](../resources/personresponsibility.md) .</span><span class="sxs-lookup"><span data-stu-id="fc78c-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="fc78c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [personResponsibility](../resources/personresponsibility.md).</span><span class="sxs-lookup"><span data-stu-id="fc78c-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="fc78c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc78c-130">Property</span></span>|<span data-ttu-id="fc78c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc78c-131">Type</span></span>|<span data-ttu-id="fc78c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc78c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc78c-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="fc78c-133">allowedAudiences</span></span>|<span data-ttu-id="fc78c-134">String</span><span class="sxs-lookup"><span data-stu-id="fc78c-134">String</span></span>|<span data-ttu-id="fc78c-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="fc78c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="fc78c-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fc78c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="fc78c-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fc78c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fc78c-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="fc78c-138">collaborationTags</span></span>|<span data-ttu-id="fc78c-139">Coleção String</span><span class="sxs-lookup"><span data-stu-id="fc78c-139">String collection</span></span>|<span data-ttu-id="fc78c-140">Contém marcas de cenário de experiência que um usuário associou aos juros.</span><span class="sxs-lookup"><span data-stu-id="fc78c-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="fc78c-141">Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="fc78c-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="fc78c-142">description</span><span class="sxs-lookup"><span data-stu-id="fc78c-142">description</span></span>|<span data-ttu-id="fc78c-143">String</span><span class="sxs-lookup"><span data-stu-id="fc78c-143">String</span></span>|<span data-ttu-id="fc78c-144">Descrição da responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="fc78c-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="fc78c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fc78c-145">displayName</span></span>|<span data-ttu-id="fc78c-146">String</span><span class="sxs-lookup"><span data-stu-id="fc78c-146">String</span></span>|<span data-ttu-id="fc78c-147">Contém um nome amigável para a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="fc78c-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="fc78c-148">fracassa</span><span class="sxs-lookup"><span data-stu-id="fc78c-148">inference</span></span>|[<span data-ttu-id="fc78c-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="fc78c-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="fc78c-150">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="fc78c-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="fc78c-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="fc78c-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fc78c-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="fc78c-152">webUrl</span></span>|<span data-ttu-id="fc78c-153">String</span><span class="sxs-lookup"><span data-stu-id="fc78c-153">String</span></span>|<span data-ttu-id="fc78c-154">Contém um link para uma página da Web ou recurso sobre a responsabilidade.</span><span class="sxs-lookup"><span data-stu-id="fc78c-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="fc78c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc78c-155">Response</span></span>

<span data-ttu-id="fc78c-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personResponsibility](../resources/personresponsibility.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc78c-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc78c-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc78c-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc78c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc78c-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="fc78c-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc78c-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fc78c-160">C#</span><span class="sxs-lookup"><span data-stu-id="fc78c-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc78c-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc78c-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc78c-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc78c-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fc78c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc78c-163">Response</span></span>
<span data-ttu-id="fc78c-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fc78c-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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


