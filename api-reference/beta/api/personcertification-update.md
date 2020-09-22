---
title: Atualizar personCertification
description: Atualiza as propriedades de um objeto personCertification.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 66c6db323684d9530913e0f6675052ffca78739a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022263"
---
# <a name="update-personcertification"></a><span data-ttu-id="35b69-103">Atualizar personCertification</span><span class="sxs-lookup"><span data-stu-id="35b69-103">Update personCertification</span></span>
<span data-ttu-id="35b69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35b69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35b69-105">Atualiza as propriedades de um objeto [personCertification](../resources/personcertification.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="35b69-105">Update the properties of a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35b69-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35b69-106">Permissions</span></span>

<span data-ttu-id="35b69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35b69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35b69-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35b69-109">Permission type</span></span>                        | <span data-ttu-id="35b69-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35b69-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="35b69-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35b69-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="35b69-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="35b69-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="35b69-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35b69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35b69-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="35b69-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="35b69-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35b69-115">Application</span></span>                            | <span data-ttu-id="35b69-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35b69-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="35b69-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35b69-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/certifications/{id}
PATCH /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35b69-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35b69-118">Request headers</span></span>
|<span data-ttu-id="35b69-119">Nome</span><span class="sxs-lookup"><span data-stu-id="35b69-119">Name</span></span>|<span data-ttu-id="35b69-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35b69-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="35b69-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="35b69-121">Authorization</span></span>|<span data-ttu-id="35b69-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35b69-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="35b69-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35b69-124">Content-Type</span></span>|<span data-ttu-id="35b69-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35b69-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35b69-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35b69-127">Request body</span></span>

<span data-ttu-id="35b69-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="35b69-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="35b69-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="35b69-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="35b69-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="35b69-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="35b69-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35b69-131">Property</span></span>|<span data-ttu-id="35b69-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="35b69-132">Type</span></span>|<span data-ttu-id="35b69-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="35b69-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b69-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="35b69-134">allowedAudiences</span></span>|<span data-ttu-id="35b69-135">String</span><span class="sxs-lookup"><span data-stu-id="35b69-135">String</span></span>|<span data-ttu-id="35b69-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="35b69-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="35b69-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="35b69-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="35b69-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="35b69-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="35b69-139">Certification</span><span class="sxs-lookup"><span data-stu-id="35b69-139">certificationId</span></span>  |<span data-ttu-id="35b69-140">String</span><span class="sxs-lookup"><span data-stu-id="35b69-140">String</span></span>      |<span data-ttu-id="35b69-141">O identificador de referência para a certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-141">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="35b69-142">description</span><span class="sxs-lookup"><span data-stu-id="35b69-142">description</span></span>      |<span data-ttu-id="35b69-143">String</span><span class="sxs-lookup"><span data-stu-id="35b69-143">String</span></span>      |<span data-ttu-id="35b69-144">Descrição da certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-144">Description of the certification.</span></span>                   |
|<span data-ttu-id="35b69-145">displayName</span><span class="sxs-lookup"><span data-stu-id="35b69-145">displayName</span></span>      |<span data-ttu-id="35b69-146">String</span><span class="sxs-lookup"><span data-stu-id="35b69-146">String</span></span>      |<span data-ttu-id="35b69-147">Título da certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-147">Title of the certification.</span></span>                         |
|<span data-ttu-id="35b69-148">endDate</span><span class="sxs-lookup"><span data-stu-id="35b69-148">endDate</span></span>          |<span data-ttu-id="35b69-149">Data</span><span class="sxs-lookup"><span data-stu-id="35b69-149">Date</span></span>        |<span data-ttu-id="35b69-150">A data em que a certificação expira.</span><span class="sxs-lookup"><span data-stu-id="35b69-150">The date that the certification expires.</span></span>            |
|<span data-ttu-id="35b69-151">fracassa</span><span class="sxs-lookup"><span data-stu-id="35b69-151">inference</span></span>|[<span data-ttu-id="35b69-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="35b69-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="35b69-153">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="35b69-154">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="35b69-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="35b69-155">issuedDate</span><span class="sxs-lookup"><span data-stu-id="35b69-155">issuedDate</span></span>       |<span data-ttu-id="35b69-156">Data</span><span class="sxs-lookup"><span data-stu-id="35b69-156">Date</span></span>        |<span data-ttu-id="35b69-157">A data em que a certificação foi emitida.</span><span class="sxs-lookup"><span data-stu-id="35b69-157">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="35b69-158">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="35b69-158">issuingAuthority</span></span> |<span data-ttu-id="35b69-159">String</span><span class="sxs-lookup"><span data-stu-id="35b69-159">String</span></span>      |<span data-ttu-id="35b69-160">Autoridade que atribuiu a certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-160">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="35b69-161">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="35b69-161">issuingCompany</span></span>   |<span data-ttu-id="35b69-162">String</span><span class="sxs-lookup"><span data-stu-id="35b69-162">String</span></span>      |<span data-ttu-id="35b69-163">Autoridade que atribuiu a certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-163">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="35b69-164">startDate</span><span class="sxs-lookup"><span data-stu-id="35b69-164">startDate</span></span>        |<span data-ttu-id="35b69-165">Data</span><span class="sxs-lookup"><span data-stu-id="35b69-165">Date</span></span>        |<span data-ttu-id="35b69-166">A data em que a certificação se tornou válida.</span><span class="sxs-lookup"><span data-stu-id="35b69-166">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="35b69-167">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="35b69-167">thumbnailUrl</span></span>     |<span data-ttu-id="35b69-168">String</span><span class="sxs-lookup"><span data-stu-id="35b69-168">String</span></span>      |<span data-ttu-id="35b69-169">URL que faz referência a uma miniatura da certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-169">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="35b69-170">webUrl</span><span class="sxs-lookup"><span data-stu-id="35b69-170">webUrl</span></span>           |<span data-ttu-id="35b69-171">String</span><span class="sxs-lookup"><span data-stu-id="35b69-171">String</span></span>      |<span data-ttu-id="35b69-172">URL que faz referência à certificação.</span><span class="sxs-lookup"><span data-stu-id="35b69-172">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="35b69-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="35b69-173">Response</span></span>

<span data-ttu-id="35b69-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personCertification](../resources/personcertification.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35b69-174">If successful, this method returns a `200 OK` response code and an updated [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35b69-175">Exemplos</span><span class="sxs-lookup"><span data-stu-id="35b69-175">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35b69-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35b69-176">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="35b69-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="35b69-177">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="35b69-178">C#</span><span class="sxs-lookup"><span data-stu-id="35b69-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35b69-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35b69-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35b69-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35b69-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="35b69-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="35b69-181">Response</span></span>
<span data-ttu-id="35b69-182">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="35b69-182">**Note:** The response object shown here might be shortened for readability.</span></span>
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


