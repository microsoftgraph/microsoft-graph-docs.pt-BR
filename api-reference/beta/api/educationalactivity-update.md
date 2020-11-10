---
title: Atualizar educationalactivity
description: Atualiza as propriedades de um objeto educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e672c1259d888b8a8fa4f6972268216ed57d9bdc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966639"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="d4694-103">Atualizar educationalactivity</span><span class="sxs-lookup"><span data-stu-id="d4694-103">Update educationalactivity</span></span>

<span data-ttu-id="d4694-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4694-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4694-105">Atualizar as propriedades de um objeto [educationalActivity](../resources/educationalactivity.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d4694-105">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4694-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4694-106">Permissions</span></span>

<span data-ttu-id="d4694-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4694-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4694-109">Permission type</span></span>                        | <span data-ttu-id="d4694-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4694-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4694-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4694-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4694-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d4694-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d4694-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4694-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4694-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d4694-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d4694-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4694-115">Application</span></span>                            | <span data-ttu-id="d4694-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4694-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d4694-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4694-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id}
PATCH /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d4694-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4694-118">Request headers</span></span>

| <span data-ttu-id="d4694-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d4694-119">Name</span></span>           |<span data-ttu-id="d4694-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4694-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d4694-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4694-121">Authorization</span></span>  | <span data-ttu-id="d4694-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4694-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d4694-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4694-124">Content-Type</span></span>   | <span data-ttu-id="d4694-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4694-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4694-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4694-127">Request body</span></span>

<span data-ttu-id="d4694-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d4694-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d4694-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d4694-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d4694-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d4694-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d4694-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4694-131">Property</span></span>|<span data-ttu-id="d4694-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4694-132">Type</span></span>|<span data-ttu-id="d4694-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4694-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4694-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d4694-134">allowedAudiences</span></span>|<span data-ttu-id="d4694-135">String</span><span class="sxs-lookup"><span data-stu-id="d4694-135">String</span></span>|<span data-ttu-id="d4694-136">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="d4694-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d4694-137">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d4694-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d4694-138">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d4694-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d4694-139">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="d4694-139">completionMonthYear</span></span>|<span data-ttu-id="d4694-140">Data</span><span class="sxs-lookup"><span data-stu-id="d4694-140">Date</span></span>|<span data-ttu-id="d4694-141">O mês e o ano em que o usuário formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="d4694-141">The month and year the user graduated or completed the activity.</span></span> |
|<span data-ttu-id="d4694-142">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="d4694-142">endMonthYear</span></span>|<span data-ttu-id="d4694-143">Data</span><span class="sxs-lookup"><span data-stu-id="d4694-143">Date</span></span>|<span data-ttu-id="d4694-144">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="d4694-144">The month and year the user completed the educational activity referenced.</span></span>|
|<span data-ttu-id="d4694-145">fracassa</span><span class="sxs-lookup"><span data-stu-id="d4694-145">inference</span></span>|[<span data-ttu-id="d4694-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d4694-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d4694-147">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="d4694-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d4694-148">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d4694-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d4694-149">instituição</span><span class="sxs-lookup"><span data-stu-id="d4694-149">institution</span></span>|[<span data-ttu-id="d4694-150">institutionData</span><span class="sxs-lookup"><span data-stu-id="d4694-150">institutionData</span></span>](../resources/institutiondata.md)|<span data-ttu-id="d4694-151">Contém detalhes da instituição estudada em.</span><span class="sxs-lookup"><span data-stu-id="d4694-151">Contains details of the institution studied at.</span></span> |
|<span data-ttu-id="d4694-152">programa</span><span class="sxs-lookup"><span data-stu-id="d4694-152">program</span></span>|[<span data-ttu-id="d4694-153">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d4694-153">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md)|<span data-ttu-id="d4694-154">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="d4694-154">Contains extended information about the program or course.</span></span>|
|<span data-ttu-id="d4694-155">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="d4694-155">startMonthYear</span></span>|<span data-ttu-id="d4694-156">Data</span><span class="sxs-lookup"><span data-stu-id="d4694-156">Date</span></span>|<span data-ttu-id="d4694-157">O mês e o ano em que o usuário tiver iniciado a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="d4694-157">The month and year the user commenced the activity referenced.</span></span>|

## <a name="response"></a><span data-ttu-id="d4694-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4694-158">Response</span></span>

<span data-ttu-id="d4694-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationalActivity](../resources/educationalactivity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4694-159">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4694-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4694-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4694-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4694-161">Request</span></span>

<span data-ttu-id="d4694-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4694-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4694-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4694-163">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
Content-type: application/json

{
  "institution": {
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    }
  }
}
```

# <a name="c"></a>[<span data-ttu-id="d4694-164">C#</span><span class="sxs-lookup"><span data-stu-id="d4694-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4694-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4694-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4694-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4694-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4694-167">Java</span><span class="sxs-lookup"><span data-stu-id="d4694-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationalactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d4694-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4694-168">Response</span></span>

<span data-ttu-id="d4694-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4694-169">The following is an example of the response.</span></span>

> <span data-ttu-id="d4694-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4694-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
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


