---
title: Atualizar personAnnotation
description: Atualiza as propriedades de um objeto personAnnotation.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e6a0b2db3abfd2bc1707815fd936f45a8cbd5d11
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809578"
---
# <a name="update-personannotation"></a><span data-ttu-id="c3e5b-103">Atualizar personAnnotation</span><span class="sxs-lookup"><span data-stu-id="c3e5b-103">Update personAnnotation</span></span>
<span data-ttu-id="c3e5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3e5b-105">Atualiza as propriedades de um objeto [personAnnotation](../resources/personannotation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-105">Update the properties of a [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3e5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3e5b-106">Permissions</span></span>

<span data-ttu-id="c3e5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3e5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3e5b-109">Permission type</span></span>                        | <span data-ttu-id="c3e5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3e5b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="c3e5b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3e5b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3e5b-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3e5b-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c3e5b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3e5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3e5b-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3e5b-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c3e5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3e5b-115">Application</span></span>                            | <span data-ttu-id="c3e5b-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3e5b-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="c3e5b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3e5b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/notes/{id}
PATCH /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c3e5b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3e5b-118">Request headers</span></span>
|<span data-ttu-id="c3e5b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c3e5b-119">Name</span></span>|<span data-ttu-id="c3e5b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3e5b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3e5b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3e5b-121">Authorization</span></span>|<span data-ttu-id="c3e5b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3e5b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3e5b-124">Content-Type</span></span>|<span data-ttu-id="c3e5b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3e5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3e5b-127">Request body</span></span>

<span data-ttu-id="c3e5b-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c3e5b-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c3e5b-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="c3e5b-131">A tabela a seguir mostra as propriedades que são possíveis de atualizar em um objeto [personAnnotation](../resources/personannotation.md) existente no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-131">The following table shows the properties that are possible to update within an existing [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="c3e5b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3e5b-132">Property</span></span>|<span data-ttu-id="c3e5b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3e5b-133">Type</span></span>|<span data-ttu-id="c3e5b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3e5b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e5b-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="c3e5b-135">allowedAudiences</span></span>|<span data-ttu-id="c3e5b-136">String</span><span class="sxs-lookup"><span data-stu-id="c3e5b-136">String</span></span>|<span data-ttu-id="c3e5b-137">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="c3e5b-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="c3e5b-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="c3e5b-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c3e5b-140">detalhada</span><span class="sxs-lookup"><span data-stu-id="c3e5b-140">detail</span></span>|[<span data-ttu-id="c3e5b-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="c3e5b-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="c3e5b-142">Contém os detalhes da anotação propriamente dita.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-142">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="c3e5b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c3e5b-143">displayName</span></span>|<span data-ttu-id="c3e5b-144">String</span><span class="sxs-lookup"><span data-stu-id="c3e5b-144">String</span></span>|<span data-ttu-id="c3e5b-145">Contém um nome amigável para a anotação.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-145">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="c3e5b-146">fracassa</span><span class="sxs-lookup"><span data-stu-id="c3e5b-146">inference</span></span>|[<span data-ttu-id="c3e5b-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="c3e5b-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="c3e5b-148">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="c3e5b-149">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="c3e5b-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="c3e5b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3e5b-150">Response</span></span>

<span data-ttu-id="c3e5b-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personAnnotation](../resources/personannotation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-151">If successful, this method returns a `200 OK` response code and an updated [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3e5b-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3e5b-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3e5b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3e5b-153">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="c3e5b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3e5b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personannotation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/notes/{id}
Content-Type: application/json
Content-length: 413

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="c3e5b-155">C#</span><span class="sxs-lookup"><span data-stu-id="c3e5b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3e5b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3e5b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3e5b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3e5b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c3e5b-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3e5b-158">Response</span></span>
<span data-ttu-id="c3e5b-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3e5b-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
    "@odata.type": "microsoft.graph.personAnnotation"
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
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow."
  },
  "displayName": "About Me"
}
```
