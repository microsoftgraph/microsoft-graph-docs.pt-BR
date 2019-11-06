---
title: Atualizar educationalactivity
description: Atualiza as propriedades de um objeto educationalactivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 68d9c6d2499b3610361ab0fdc2b78c188853b65b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994749"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="7059d-103">Atualizar educationalactivity</span><span class="sxs-lookup"><span data-stu-id="7059d-103">Update educationalactivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7059d-104">Atualizar as propriedades de um objeto [educationalActivity](../resources/educationalactivity.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7059d-104">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7059d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7059d-105">Permissions</span></span>

<span data-ttu-id="7059d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7059d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7059d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7059d-108">Permission type</span></span>                        | <span data-ttu-id="7059d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7059d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7059d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7059d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7059d-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7059d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7059d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7059d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7059d-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7059d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7059d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7059d-114">Application</span></span>                            | <span data-ttu-id="7059d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7059d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="7059d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7059d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="7059d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7059d-117">Request headers</span></span>

| <span data-ttu-id="7059d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7059d-118">Name</span></span>           |<span data-ttu-id="7059d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7059d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7059d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7059d-120">Authorization</span></span>  | <span data-ttu-id="7059d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7059d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7059d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7059d-123">Content-Type</span></span>   | <span data-ttu-id="7059d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7059d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7059d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7059d-126">Request body</span></span>

<span data-ttu-id="7059d-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7059d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7059d-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7059d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7059d-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7059d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7059d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7059d-130">Property</span></span>           | <span data-ttu-id="7059d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7059d-131">Type</span></span>                                                                  | <span data-ttu-id="7059d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7059d-132">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="7059d-133">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="7059d-133">completionMonthYear</span></span> |<span data-ttu-id="7059d-134">Data</span><span class="sxs-lookup"><span data-stu-id="7059d-134">Date</span></span>                                                                   | <span data-ttu-id="7059d-135">O mês e o ano em que o usuário formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="7059d-135">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="7059d-136">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="7059d-136">endMonthYear</span></span>        |<span data-ttu-id="7059d-137">Data</span><span class="sxs-lookup"><span data-stu-id="7059d-137">Date</span></span>                                                                   | <span data-ttu-id="7059d-138">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="7059d-138">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="7059d-139">instituição</span><span class="sxs-lookup"><span data-stu-id="7059d-139">institution</span></span>         |[<span data-ttu-id="7059d-140">institutionData</span><span class="sxs-lookup"><span data-stu-id="7059d-140">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="7059d-141">Contém detalhes da instituição estudada em.</span><span class="sxs-lookup"><span data-stu-id="7059d-141">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="7059d-142">programa</span><span class="sxs-lookup"><span data-stu-id="7059d-142">program</span></span>             |[<span data-ttu-id="7059d-143">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="7059d-143">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="7059d-144">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="7059d-144">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="7059d-145">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="7059d-145">startMonthYear</span></span>      |<span data-ttu-id="7059d-146">Data</span><span class="sxs-lookup"><span data-stu-id="7059d-146">Date</span></span>                                                                   | <span data-ttu-id="7059d-147">O mês e o ano em que o usuário tiver iniciado a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="7059d-147">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="7059d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7059d-148">Response</span></span>

<span data-ttu-id="7059d-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationalActivity](../resources/educationalactivity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7059d-149">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7059d-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7059d-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7059d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7059d-151">Request</span></span>

<span data-ttu-id="7059d-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7059d-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7059d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="7059d-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7059d-154">C#</span><span class="sxs-lookup"><span data-stu-id="7059d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7059d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7059d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7059d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7059d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7059d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7059d-157">Response</span></span>

<span data-ttu-id="7059d-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7059d-158">The following is an example of the response.</span></span>

> <span data-ttu-id="7059d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7059d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationalactivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
