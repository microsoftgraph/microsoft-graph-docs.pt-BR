---
title: Atualizar personAward
description: Atualiza as propriedades de um objeto personAward.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1338c1990ad76611295ac34e13b30b53651839d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969316"
---
# <a name="update-personaward"></a><span data-ttu-id="bc5b0-103">Atualizar personAward</span><span class="sxs-lookup"><span data-stu-id="bc5b0-103">Update personAward</span></span>

<span data-ttu-id="bc5b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc5b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc5b0-105">Atualiza as propriedades de um objeto [personAward](../resources/personAward.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-105">Update the properties of a [personAward](../resources/personAward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc5b0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc5b0-106">Permissions</span></span>

<span data-ttu-id="bc5b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc5b0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc5b0-109">Permission type</span></span>                        | <span data-ttu-id="bc5b0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc5b0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="bc5b0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc5b0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc5b0-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bc5b0-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bc5b0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc5b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5b0-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bc5b0-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bc5b0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc5b0-115">Application</span></span>                            | <span data-ttu-id="bc5b0-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc5b0-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="bc5b0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5b0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/awards/{id}
PATCH /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bc5b0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5b0-118">Request headers</span></span>
|<span data-ttu-id="bc5b0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bc5b0-119">Name</span></span>|<span data-ttu-id="bc5b0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5b0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bc5b0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc5b0-121">Authorization</span></span>|<span data-ttu-id="bc5b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bc5b0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc5b0-124">Content-Type</span></span>|<span data-ttu-id="bc5b0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc5b0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5b0-127">Request body</span></span>

<span data-ttu-id="bc5b0-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bc5b0-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bc5b0-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="bc5b0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc5b0-131">Property</span></span>|<span data-ttu-id="bc5b0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc5b0-132">Type</span></span>|<span data-ttu-id="bc5b0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5b0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc5b0-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="bc5b0-134">allowedAudiences</span></span>|<span data-ttu-id="bc5b0-135">String</span><span class="sxs-lookup"><span data-stu-id="bc5b0-135">String</span></span>|<span data-ttu-id="bc5b0-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="bc5b0-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="bc5b0-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="bc5b0-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bc5b0-139">description</span><span class="sxs-lookup"><span data-stu-id="bc5b0-139">description</span></span>|<span data-ttu-id="bc5b0-140">String</span><span class="sxs-lookup"><span data-stu-id="bc5b0-140">String</span></span>|<span data-ttu-id="bc5b0-141">Descpription do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-141">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="bc5b0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="bc5b0-142">displayName</span></span>|<span data-ttu-id="bc5b0-143">String</span><span class="sxs-lookup"><span data-stu-id="bc5b0-143">String</span></span>|<span data-ttu-id="bc5b0-144">Nome do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-144">Name of the award or honor.</span></span> |
|<span data-ttu-id="bc5b0-145">fracassa</span><span class="sxs-lookup"><span data-stu-id="bc5b0-145">inference</span></span>|[<span data-ttu-id="bc5b0-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="bc5b0-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="bc5b0-147">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="bc5b0-148">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="bc5b0-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc5b0-149">issuedDate</span><span class="sxs-lookup"><span data-stu-id="bc5b0-149">issuedDate</span></span>|<span data-ttu-id="bc5b0-150">Data</span><span class="sxs-lookup"><span data-stu-id="bc5b0-150">Date</span></span>|<span data-ttu-id="bc5b0-151">A data em que o prêmio ou honra foi concedido.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-151">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="bc5b0-152">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="bc5b0-152">issuingAuthority</span></span>|<span data-ttu-id="bc5b0-153">String</span><span class="sxs-lookup"><span data-stu-id="bc5b0-153">String</span></span>|<span data-ttu-id="bc5b0-154">Autoridade que concedeu o prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-154">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="bc5b0-155">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="bc5b0-155">thumbnailUrl</span></span>|<span data-ttu-id="bc5b0-156">String</span><span class="sxs-lookup"><span data-stu-id="bc5b0-156">String</span></span>|<span data-ttu-id="bc5b0-157">URL que faz referência a uma miniatura do prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-157">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="bc5b0-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="bc5b0-158">webUrl</span></span>|<span data-ttu-id="bc5b0-159">String</span><span class="sxs-lookup"><span data-stu-id="bc5b0-159">String</span></span>|<span data-ttu-id="bc5b0-160">URL que faz referência ao prêmio ou honra.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-160">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="bc5b0-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5b0-161">Response</span></span>

<span data-ttu-id="bc5b0-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personAward](../resources/personaward.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-162">If successful, this method returns a `200 OK` response code and an updated [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc5b0-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc5b0-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc5b0-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5b0-164">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="bc5b0-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5b0-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personaward"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/awards/{personAwardId}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg"
}
```
# <a name="c"></a>[<span data-ttu-id="bc5b0-166">C#</span><span class="sxs-lookup"><span data-stu-id="bc5b0-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc5b0-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc5b0-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc5b0-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc5b0-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bc5b0-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5b0-169">Response</span></span>
<span data-ttu-id="bc5b0-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc5b0-170">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


