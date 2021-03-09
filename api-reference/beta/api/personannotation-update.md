---
title: Atualizar personAnnotation
description: Atualize as propriedades de um objeto personAnnotation.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5d9c6503c3aeb5fb52ad0982eabfc29729cc23e6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576054"
---
# <a name="update-personannotation"></a><span data-ttu-id="ecdff-103">Atualizar personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ecdff-103">Update personAnnotation</span></span>
<span data-ttu-id="ecdff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecdff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecdff-105">Atualize as propriedades de [um objeto personAnnotation](../resources/personannotation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="ecdff-105">Update the properties of a [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ecdff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecdff-106">Permissions</span></span>

<span data-ttu-id="ecdff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecdff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecdff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecdff-109">Permission type</span></span>                        | <span data-ttu-id="ecdff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecdff-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ecdff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecdff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecdff-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdff-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ecdff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecdff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecdff-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdff-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ecdff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecdff-115">Application</span></span>                            | <span data-ttu-id="ecdff-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdff-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ecdff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/notes/{id}
PATCH /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ecdff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdff-118">Request headers</span></span>
|<span data-ttu-id="ecdff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ecdff-119">Name</span></span>|<span data-ttu-id="ecdff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecdff-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ecdff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecdff-121">Authorization</span></span>|<span data-ttu-id="ecdff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecdff-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ecdff-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ecdff-124">Content-Type</span></span>|<span data-ttu-id="ecdff-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecdff-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecdff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdff-127">Request body</span></span>

<span data-ttu-id="ecdff-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ecdff-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ecdff-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ecdff-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ecdff-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ecdff-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="ecdff-131">A tabela a seguir mostra as propriedades que são possíveis de atualizar dentro de um [objeto personAnnotation](../resources/personannotation.md) existente no perfil de um [usuário](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="ecdff-131">The following table shows the properties that are possible to update within an existing [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="ecdff-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecdff-132">Property</span></span>|<span data-ttu-id="ecdff-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecdff-133">Type</span></span>|<span data-ttu-id="ecdff-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecdff-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecdff-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ecdff-135">allowedAudiences</span></span>|<span data-ttu-id="ecdff-136">String</span><span class="sxs-lookup"><span data-stu-id="ecdff-136">String</span></span>|<span data-ttu-id="ecdff-137">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="ecdff-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ecdff-138">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ecdff-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ecdff-139">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ecdff-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ecdff-140">detail</span><span class="sxs-lookup"><span data-stu-id="ecdff-140">detail</span></span>|[<span data-ttu-id="ecdff-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="ecdff-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="ecdff-142">Contém os detalhes da própria nota.</span><span class="sxs-lookup"><span data-stu-id="ecdff-142">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="ecdff-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ecdff-143">displayName</span></span>|<span data-ttu-id="ecdff-144">String</span><span class="sxs-lookup"><span data-stu-id="ecdff-144">String</span></span>|<span data-ttu-id="ecdff-145">Contém um nome amigável para a nota.</span><span class="sxs-lookup"><span data-stu-id="ecdff-145">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="ecdff-146">inferência</span><span class="sxs-lookup"><span data-stu-id="ecdff-146">inference</span></span>|[<span data-ttu-id="ecdff-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ecdff-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ecdff-148">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="ecdff-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ecdff-149">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ecdff-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ecdff-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecdff-150">Response</span></span>

<span data-ttu-id="ecdff-151">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto personAnnotation](../resources/personannotation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecdff-151">If successful, this method returns a `200 OK` response code and an updated [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecdff-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ecdff-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecdff-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdff-153">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="ecdff-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdff-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personannotation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/notes/{id}
Content-Type: application/json
Content-length: 413

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="ecdff-155">C#</span><span class="sxs-lookup"><span data-stu-id="ecdff-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecdff-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecdff-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecdff-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecdff-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ecdff-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecdff-158">Response</span></span>
<span data-ttu-id="ecdff-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ecdff-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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



