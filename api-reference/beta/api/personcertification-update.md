---
title: Atualizar personCertification
description: Atualiza as propriedades de um objeto personCertification.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 52327323d177e9414790583cee670d300c9095c4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809602"
---
# <a name="update-personcertification"></a><span data-ttu-id="f5ed1-103">Atualizar personCertification</span><span class="sxs-lookup"><span data-stu-id="f5ed1-103">Update personCertification</span></span>
<span data-ttu-id="f5ed1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ed1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5ed1-105">Atualiza as propriedades de um objeto [personCertification](../resources/personcertification.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-105">Update the properties of a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5ed1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5ed1-106">Permissions</span></span>

<span data-ttu-id="f5ed1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5ed1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5ed1-109">Permission type</span></span>                        | <span data-ttu-id="f5ed1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5ed1-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f5ed1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5ed1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5ed1-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f5ed1-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f5ed1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5ed1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ed1-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f5ed1-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f5ed1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5ed1-115">Application</span></span>                            | <span data-ttu-id="f5ed1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ed1-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f5ed1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ed1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/certifications/{id}
PATCH /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5ed1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ed1-118">Request headers</span></span>
|<span data-ttu-id="f5ed1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f5ed1-119">Name</span></span>|<span data-ttu-id="f5ed1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ed1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5ed1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ed1-121">Authorization</span></span>|<span data-ttu-id="f5ed1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f5ed1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5ed1-124">Content-Type</span></span>|<span data-ttu-id="f5ed1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ed1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ed1-127">Request body</span></span>

<span data-ttu-id="f5ed1-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f5ed1-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f5ed1-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="f5ed1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5ed1-131">Property</span></span>|<span data-ttu-id="f5ed1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5ed1-132">Type</span></span>|<span data-ttu-id="f5ed1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ed1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ed1-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="f5ed1-134">allowedAudiences</span></span>|<span data-ttu-id="f5ed1-135">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-135">String</span></span>|<span data-ttu-id="f5ed1-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f5ed1-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f5ed1-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f5ed1-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f5ed1-139">Certification</span><span class="sxs-lookup"><span data-stu-id="f5ed1-139">certificationId</span></span>  |<span data-ttu-id="f5ed1-140">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-140">String</span></span>      |<span data-ttu-id="f5ed1-141">O identificador de referência para a certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-141">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="f5ed1-142">description</span><span class="sxs-lookup"><span data-stu-id="f5ed1-142">description</span></span>      |<span data-ttu-id="f5ed1-143">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-143">String</span></span>      |<span data-ttu-id="f5ed1-144">Descrição da certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-144">Description of the certification.</span></span>                   |
|<span data-ttu-id="f5ed1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f5ed1-145">displayName</span></span>      |<span data-ttu-id="f5ed1-146">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-146">String</span></span>      |<span data-ttu-id="f5ed1-147">Título da certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-147">Title of the certification.</span></span>                         |
|<span data-ttu-id="f5ed1-148">endDate</span><span class="sxs-lookup"><span data-stu-id="f5ed1-148">endDate</span></span>          |<span data-ttu-id="f5ed1-149">Data</span><span class="sxs-lookup"><span data-stu-id="f5ed1-149">Date</span></span>        |<span data-ttu-id="f5ed1-150">A data em que a certificação expira.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-150">The date that the certification expires.</span></span>            |
|<span data-ttu-id="f5ed1-151">fracassa</span><span class="sxs-lookup"><span data-stu-id="f5ed1-151">inference</span></span>|[<span data-ttu-id="f5ed1-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="f5ed1-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f5ed1-153">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f5ed1-154">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f5ed1-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f5ed1-155">issuedDate</span><span class="sxs-lookup"><span data-stu-id="f5ed1-155">issuedDate</span></span>       |<span data-ttu-id="f5ed1-156">Data</span><span class="sxs-lookup"><span data-stu-id="f5ed1-156">Date</span></span>        |<span data-ttu-id="f5ed1-157">A data em que a certificação foi emitida.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-157">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="f5ed1-158">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="f5ed1-158">issuingAuthority</span></span> |<span data-ttu-id="f5ed1-159">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-159">String</span></span>      |<span data-ttu-id="f5ed1-160">Autoridade que atribuiu a certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-160">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="f5ed1-161">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="f5ed1-161">issuingCompany</span></span>   |<span data-ttu-id="f5ed1-162">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-162">String</span></span>      |<span data-ttu-id="f5ed1-163">Autoridade que atribuiu a certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-163">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="f5ed1-164">startDate</span><span class="sxs-lookup"><span data-stu-id="f5ed1-164">startDate</span></span>        |<span data-ttu-id="f5ed1-165">Data</span><span class="sxs-lookup"><span data-stu-id="f5ed1-165">Date</span></span>        |<span data-ttu-id="f5ed1-166">A data em que a certificação se tornou válida.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-166">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="f5ed1-167">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="f5ed1-167">thumbnailUrl</span></span>     |<span data-ttu-id="f5ed1-168">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-168">String</span></span>      |<span data-ttu-id="f5ed1-169">URL que faz referência a uma miniatura da certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-169">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="f5ed1-170">webUrl</span><span class="sxs-lookup"><span data-stu-id="f5ed1-170">webUrl</span></span>           |<span data-ttu-id="f5ed1-171">String</span><span class="sxs-lookup"><span data-stu-id="f5ed1-171">String</span></span>      |<span data-ttu-id="f5ed1-172">URL que faz referência à certificação.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-172">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="f5ed1-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ed1-173">Response</span></span>

<span data-ttu-id="f5ed1-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personCertification](../resources/personcertification.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-174">If successful, this method returns a `200 OK` response code and an updated [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5ed1-175">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5ed1-175">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5ed1-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ed1-176">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="f5ed1-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ed1-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personcertification"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/certifications/{id}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence"
}
```
# <a name="c"></a>[<span data-ttu-id="f5ed1-178">C#</span><span class="sxs-lookup"><span data-stu-id="f5ed1-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5ed1-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5ed1-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5ed1-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5ed1-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f5ed1-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ed1-181">Response</span></span>
<span data-ttu-id="f5ed1-182">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f5ed1-182">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence",
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
