---
title: Criar educationalActivity
description: Crie uma nova educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 366417fd6cf8e218bf7fc3a0fe2f14bc9c0ac4d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036937"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="b6c52-103">Criar educationalActivity</span><span class="sxs-lookup"><span data-stu-id="b6c52-103">Create educationalActivity</span></span>

<span data-ttu-id="b6c52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6c52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c52-105">Crie uma nova [educationalActivity](../resources/educationalactivity.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="b6c52-105">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6c52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6c52-106">Permissions</span></span>

<span data-ttu-id="b6c52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6c52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6c52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6c52-109">Permission type</span></span>                        | <span data-ttu-id="b6c52-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6c52-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b6c52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6c52-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6c52-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c52-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b6c52-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6c52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6c52-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c52-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b6c52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6c52-115">Application</span></span>                            | <span data-ttu-id="b6c52-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c52-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b6c52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6c52-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/educationalActivities
POST /users/{id | userPrincipalName}/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="b6c52-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6c52-118">Request headers</span></span>

| <span data-ttu-id="b6c52-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b6c52-119">Name</span></span>           |<span data-ttu-id="b6c52-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6c52-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b6c52-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6c52-121">Authorization</span></span>  | <span data-ttu-id="b6c52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6c52-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b6c52-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6c52-124">Content-Type</span></span>   | <span data-ttu-id="b6c52-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6c52-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6c52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6c52-127">Request body</span></span>

<span data-ttu-id="b6c52-128">No corpo da solicitação, fornece uma representação JSON de um [objeto educationalActivity.](../resources/educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="b6c52-128">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

<span data-ttu-id="b6c52-129">A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto [educationalActivity](../resources/educationalactivity.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="b6c52-129">The following table shows the properties that are possible to set when creating a new [educationalActivity](../resources/educationalactivity.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="b6c52-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6c52-130">Property</span></span>|<span data-ttu-id="b6c52-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6c52-131">Type</span></span>|<span data-ttu-id="b6c52-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6c52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6c52-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="b6c52-133">allowedAudiences</span></span>|<span data-ttu-id="b6c52-134">String</span><span class="sxs-lookup"><span data-stu-id="b6c52-134">String</span></span>|<span data-ttu-id="b6c52-135">As audiências que são capazes de ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="b6c52-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b6c52-136">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b6c52-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b6c52-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b6c52-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b6c52-138">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="b6c52-138">completionMonthYear</span></span>|<span data-ttu-id="b6c52-139">Date</span><span class="sxs-lookup"><span data-stu-id="b6c52-139">Date</span></span>|<span data-ttu-id="b6c52-140">O mês e o ano em que o usuário se formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="b6c52-140">The month and year the user graduated or completed the activity.</span></span> |
|<span data-ttu-id="b6c52-141">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="b6c52-141">endMonthYear</span></span>|<span data-ttu-id="b6c52-142">Date</span><span class="sxs-lookup"><span data-stu-id="b6c52-142">Date</span></span>|<span data-ttu-id="b6c52-143">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="b6c52-143">The month and year the user completed the educational activity referenced.</span></span>|
|<span data-ttu-id="b6c52-144">inferência</span><span class="sxs-lookup"><span data-stu-id="b6c52-144">inference</span></span>|[<span data-ttu-id="b6c52-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="b6c52-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b6c52-146">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="b6c52-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b6c52-147">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b6c52-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b6c52-148">institution</span><span class="sxs-lookup"><span data-stu-id="b6c52-148">institution</span></span>|[<span data-ttu-id="b6c52-149">institutionData</span><span class="sxs-lookup"><span data-stu-id="b6c52-149">institutionData</span></span>](../resources/institutiondata.md)|<span data-ttu-id="b6c52-150">Contém detalhes da instituição em que estudou.</span><span class="sxs-lookup"><span data-stu-id="b6c52-150">Contains details of the institution studied at.</span></span> |
|<span data-ttu-id="b6c52-151">program</span><span class="sxs-lookup"><span data-stu-id="b6c52-151">program</span></span>|[<span data-ttu-id="b6c52-152">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="b6c52-152">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md)|<span data-ttu-id="b6c52-153">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="b6c52-153">Contains extended information about the program or course.</span></span>|
|<span data-ttu-id="b6c52-154">source</span><span class="sxs-lookup"><span data-stu-id="b6c52-154">source</span></span>|[<span data-ttu-id="b6c52-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="b6c52-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="b6c52-156">Onde os valores se originaram se sincronizados de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="b6c52-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="b6c52-157">Herdado [do itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b6c52-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b6c52-158">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="b6c52-158">startMonthYear</span></span>|<span data-ttu-id="b6c52-159">Date</span><span class="sxs-lookup"><span data-stu-id="b6c52-159">Date</span></span>|<span data-ttu-id="b6c52-160">O mês e o ano em que o usuário iniciou a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="b6c52-160">The month and year the user commenced the activity referenced.</span></span>|

## <a name="response"></a><span data-ttu-id="b6c52-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6c52-161">Response</span></span>

<span data-ttu-id="b6c52-162">Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo objeto [educationalActivity](../resources/educationalactivity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6c52-162">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6c52-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6c52-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6c52-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6c52-164">Request</span></span>

<span data-ttu-id="b6c52-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6c52-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6c52-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6c52-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "description": null,
    "displayName": "Colorado State University",
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    },
    "webUrl": "https://www.colostate.edu"
  },
  "program": {
    "abbreviation": "MBA",
    "activities": null,
    "awards": null,
    "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
    "displayName": "Master of Business Administration",
    "fieldsOfStudy": null,
    "grade": "3.9",
    "notes": null,
    "webUrl": "https://biz.colostate.edu"
  },
  "startMonthYear": "Date"
}
```
# <a name="c"></a>[<span data-ttu-id="b6c52-167">C#</span><span class="sxs-lookup"><span data-stu-id="b6c52-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationalactivity-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6c52-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6c52-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationalactivity-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6c52-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6c52-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationalactivity-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6c52-170">Java</span><span class="sxs-lookup"><span data-stu-id="b6c52-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationalactivity-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6c52-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6c52-171">Response</span></span>

<span data-ttu-id="b6c52-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6c52-172">The following is an example of the response.</span></span>

> <span data-ttu-id="b6c52-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6c52-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "description": null,
    "displayName": "Colorado State University",
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    },
    "webUrl": "https://www.colostate.edu"
  },
  "program": {
    "abbreviation": "MBA",
    "activities": null,
    "awards": null,
    "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
    "displayName": "Master of Business Administration",
    "fieldsOfStudy": null,
    "grade": "3.9",
    "notes": null,
    "webUrl": "https://biz.colostate.edu"
  },
  "startMonthYear": "Date"
}
```


