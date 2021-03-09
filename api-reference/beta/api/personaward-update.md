---
title: Atualizar personAward
description: Atualize as propriedades de um objeto personAward.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 821293e804b5ec56cdde33464695ad0dcec7a103
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574019"
---
# <a name="update-personaward"></a><span data-ttu-id="8c3b5-103">Atualizar personAward</span><span class="sxs-lookup"><span data-stu-id="8c3b5-103">Update personAward</span></span>

<span data-ttu-id="8c3b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c3b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c3b5-105">Atualize as propriedades de [um objeto personAward](../resources/personAward.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="8c3b5-105">Update the properties of a [personAward](../resources/personAward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c3b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c3b5-106">Permissions</span></span>

<span data-ttu-id="8c3b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c3b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c3b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c3b5-109">Permission type</span></span>                        | <span data-ttu-id="8c3b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c3b5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8c3b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c3b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c3b5-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c3b5-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8c3b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c3b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c3b5-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c3b5-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8c3b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c3b5-115">Application</span></span>                            | <span data-ttu-id="8c3b5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c3b5-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="8c3b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c3b5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/awards/{id}
PATCH /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8c3b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c3b5-118">Request headers</span></span>
|<span data-ttu-id="8c3b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8c3b5-119">Name</span></span>|<span data-ttu-id="8c3b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c3b5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c3b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c3b5-121">Authorization</span></span>|<span data-ttu-id="8c3b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8c3b5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c3b5-124">Content-Type</span></span>|<span data-ttu-id="8c3b5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c3b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c3b5-127">Request body</span></span>

<span data-ttu-id="8c3b5-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8c3b5-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8c3b5-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="8c3b5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c3b5-131">Property</span></span>|<span data-ttu-id="8c3b5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c3b5-132">Type</span></span>|<span data-ttu-id="8c3b5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c3b5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c3b5-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8c3b5-134">allowedAudiences</span></span>|<span data-ttu-id="8c3b5-135">String</span><span class="sxs-lookup"><span data-stu-id="8c3b5-135">String</span></span>|<span data-ttu-id="8c3b5-136">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8c3b5-137">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8c3b5-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8c3b5-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8c3b5-139">description</span><span class="sxs-lookup"><span data-stu-id="8c3b5-139">description</span></span>|<span data-ttu-id="8c3b5-140">String</span><span class="sxs-lookup"><span data-stu-id="8c3b5-140">String</span></span>|<span data-ttu-id="8c3b5-141">Descpription of the award or honor.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-141">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="8c3b5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8c3b5-142">displayName</span></span>|<span data-ttu-id="8c3b5-143">String</span><span class="sxs-lookup"><span data-stu-id="8c3b5-143">String</span></span>|<span data-ttu-id="8c3b5-144">Nome do prêmio ou da honra.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-144">Name of the award or honor.</span></span> |
|<span data-ttu-id="8c3b5-145">inferência</span><span class="sxs-lookup"><span data-stu-id="8c3b5-145">inference</span></span>|[<span data-ttu-id="8c3b5-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8c3b5-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8c3b5-147">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8c3b5-148">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8c3b5-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8c3b5-149">issuedDate</span><span class="sxs-lookup"><span data-stu-id="8c3b5-149">issuedDate</span></span>|<span data-ttu-id="8c3b5-150">Data</span><span class="sxs-lookup"><span data-stu-id="8c3b5-150">Date</span></span>|<span data-ttu-id="8c3b5-151">A data em que o prêmio ou a honra foi concedido.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-151">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="8c3b5-152">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="8c3b5-152">issuingAuthority</span></span>|<span data-ttu-id="8c3b5-153">String</span><span class="sxs-lookup"><span data-stu-id="8c3b5-153">String</span></span>|<span data-ttu-id="8c3b5-154">Autoridade que concedeu o prêmio ou a honra.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-154">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="8c3b5-155">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="8c3b5-155">thumbnailUrl</span></span>|<span data-ttu-id="8c3b5-156">String</span><span class="sxs-lookup"><span data-stu-id="8c3b5-156">String</span></span>|<span data-ttu-id="8c3b5-157">URL fazendo referência a uma miniatura do prêmio ou da honra.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-157">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="8c3b5-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="8c3b5-158">webUrl</span></span>|<span data-ttu-id="8c3b5-159">String</span><span class="sxs-lookup"><span data-stu-id="8c3b5-159">String</span></span>|<span data-ttu-id="8c3b5-160">URL referenciando o prêmio ou a honra.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-160">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="8c3b5-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c3b5-161">Response</span></span>

<span data-ttu-id="8c3b5-162">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto personAward](../resources/personaward.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-162">If successful, this method returns a `200 OK` response code and an updated [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c3b5-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8c3b5-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c3b5-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c3b5-164">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="8c3b5-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c3b5-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personaward"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/awards/{personAwardId}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg"
}
```
# <a name="c"></a>[<span data-ttu-id="8c3b5-166">C#</span><span class="sxs-lookup"><span data-stu-id="8c3b5-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c3b5-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c3b5-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c3b5-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c3b5-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8c3b5-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c3b5-169">Response</span></span>
<span data-ttu-id="8c3b5-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c3b5-170">**Note:** The response object shown here might be shortened for readability.</span></span>
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


