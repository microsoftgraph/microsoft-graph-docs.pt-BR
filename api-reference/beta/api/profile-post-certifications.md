---
title: Criar certificações
description: Criar um novo objeto certificações.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c0ee67610b7b7d600ec9e61d085d77c0f56e71eb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967254"
---
# <a name="create-personcertification"></a><span data-ttu-id="ab070-103">Criar personCertification</span><span class="sxs-lookup"><span data-stu-id="ab070-103">Create personCertification</span></span>
<span data-ttu-id="ab070-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab070-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab070-105">Criar um novo objeto [personCertification](../resources/personcertification.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ab070-105">Create a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab070-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab070-106">Permissions</span></span>

<span data-ttu-id="ab070-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab070-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab070-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab070-109">Permission type</span></span>                        | <span data-ttu-id="ab070-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab070-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ab070-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab070-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab070-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab070-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ab070-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab070-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab070-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab070-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ab070-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab070-115">Application</span></span>                            | <span data-ttu-id="ab070-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab070-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="ab070-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab070-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a><span data-ttu-id="ab070-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab070-118">Request headers</span></span>
|<span data-ttu-id="ab070-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ab070-119">Name</span></span>|<span data-ttu-id="ab070-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab070-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ab070-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab070-121">Authorization</span></span>|<span data-ttu-id="ab070-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab070-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ab070-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab070-124">Content-Type</span></span>|<span data-ttu-id="ab070-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab070-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab070-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab070-127">Request body</span></span>
<span data-ttu-id="ab070-128">No corpo da solicitação, forneça uma representação JSON do objeto [personCertification](../resources/personcertification.md) .</span><span class="sxs-lookup"><span data-stu-id="ab070-128">In the request body, supply a JSON representation of the [personCertification](../resources/personcertification.md) object.</span></span>

<span data-ttu-id="ab070-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto [personCertification](../resources/personcertification.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ab070-129">The following table shows the properties that are possible to set when creating a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="ab070-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab070-130">Property</span></span>|<span data-ttu-id="ab070-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab070-131">Type</span></span>|<span data-ttu-id="ab070-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab070-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab070-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ab070-133">allowedAudiences</span></span>|<span data-ttu-id="ab070-134">String</span><span class="sxs-lookup"><span data-stu-id="ab070-134">String</span></span>|<span data-ttu-id="ab070-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="ab070-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ab070-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ab070-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ab070-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ab070-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ab070-138">Certification</span><span class="sxs-lookup"><span data-stu-id="ab070-138">certificationId</span></span>  |<span data-ttu-id="ab070-139">String</span><span class="sxs-lookup"><span data-stu-id="ab070-139">String</span></span>      |<span data-ttu-id="ab070-140">O identificador de referência para a certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-140">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="ab070-141">description</span><span class="sxs-lookup"><span data-stu-id="ab070-141">description</span></span>      |<span data-ttu-id="ab070-142">String</span><span class="sxs-lookup"><span data-stu-id="ab070-142">String</span></span>      |<span data-ttu-id="ab070-143">Descrição da certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-143">Description of the certification.</span></span>                   |
|<span data-ttu-id="ab070-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ab070-144">displayName</span></span>      |<span data-ttu-id="ab070-145">String</span><span class="sxs-lookup"><span data-stu-id="ab070-145">String</span></span>      |<span data-ttu-id="ab070-146">Título da certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-146">Title of the certification.</span></span>                         |
|<span data-ttu-id="ab070-147">endDate</span><span class="sxs-lookup"><span data-stu-id="ab070-147">endDate</span></span>          |<span data-ttu-id="ab070-148">Data</span><span class="sxs-lookup"><span data-stu-id="ab070-148">Date</span></span>        |<span data-ttu-id="ab070-149">A data em que a certificação expira.</span><span class="sxs-lookup"><span data-stu-id="ab070-149">The date that the certification expires.</span></span>            |
|<span data-ttu-id="ab070-150">fracassa</span><span class="sxs-lookup"><span data-stu-id="ab070-150">inference</span></span>|[<span data-ttu-id="ab070-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ab070-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ab070-152">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ab070-153">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ab070-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ab070-154">issuedDate</span><span class="sxs-lookup"><span data-stu-id="ab070-154">issuedDate</span></span>       |<span data-ttu-id="ab070-155">Data</span><span class="sxs-lookup"><span data-stu-id="ab070-155">Date</span></span>        |<span data-ttu-id="ab070-156">A data em que a certificação foi emitida.</span><span class="sxs-lookup"><span data-stu-id="ab070-156">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="ab070-157">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="ab070-157">issuingAuthority</span></span> |<span data-ttu-id="ab070-158">String</span><span class="sxs-lookup"><span data-stu-id="ab070-158">String</span></span>      |<span data-ttu-id="ab070-159">Autoridade que atribuiu a certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-159">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="ab070-160">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="ab070-160">issuingCompany</span></span>   |<span data-ttu-id="ab070-161">String</span><span class="sxs-lookup"><span data-stu-id="ab070-161">String</span></span>      |<span data-ttu-id="ab070-162">Autoridade que atribuiu a certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-162">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="ab070-163">source</span><span class="sxs-lookup"><span data-stu-id="ab070-163">source</span></span>|[<span data-ttu-id="ab070-164">personDataSource</span><span class="sxs-lookup"><span data-stu-id="ab070-164">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ab070-165">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="ab070-165">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ab070-166">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ab070-166">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ab070-167">startDate</span><span class="sxs-lookup"><span data-stu-id="ab070-167">startDate</span></span>        |<span data-ttu-id="ab070-168">Data</span><span class="sxs-lookup"><span data-stu-id="ab070-168">Date</span></span>        |<span data-ttu-id="ab070-169">A data em que a certificação se tornou válida.</span><span class="sxs-lookup"><span data-stu-id="ab070-169">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="ab070-170">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="ab070-170">thumbnailUrl</span></span>     |<span data-ttu-id="ab070-171">String</span><span class="sxs-lookup"><span data-stu-id="ab070-171">String</span></span>      |<span data-ttu-id="ab070-172">URL que faz referência a uma miniatura da certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-172">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="ab070-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="ab070-173">webUrl</span></span>           |<span data-ttu-id="ab070-174">String</span><span class="sxs-lookup"><span data-stu-id="ab070-174">String</span></span>      |<span data-ttu-id="ab070-175">URL que faz referência à certificação.</span><span class="sxs-lookup"><span data-stu-id="ab070-175">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="ab070-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab070-176">Response</span></span>

<span data-ttu-id="ab070-177">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personCertification](../resources/personcertification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab070-177">If successful, this method returns a `201 Created` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab070-178">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab070-178">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="ab070-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab070-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personCertification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/certifications
Content-Type: application/json
Content-length: 497

{
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
# <a name="c"></a>[<span data-ttu-id="ab070-180">C#</span><span class="sxs-lookup"><span data-stu-id="ab070-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personcertification-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab070-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab070-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personcertification-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab070-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab070-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personcertification-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab070-183">Java</span><span class="sxs-lookup"><span data-stu-id="ab070-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personcertification-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ab070-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab070-184">Response</span></span>
<span data-ttu-id="ab070-185">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab070-185">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": null,
  "issuingCompany": null,
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```


