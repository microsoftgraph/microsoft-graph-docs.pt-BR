---
title: Atualizar educationalactivity
description: Atualiza as propriedades de um objeto educationalactivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e044bfc8950965cdde51deeab0c3e2e2cae4d396
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427848"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="9fc9a-103">Atualizar educationalactivity</span><span class="sxs-lookup"><span data-stu-id="9fc9a-103">Update educationalactivity</span></span>

<span data-ttu-id="9fc9a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9fc9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc9a-105">Atualizar as propriedades de um objeto [educationalActivity](../resources/educationalactivity.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-105">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9fc9a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fc9a-106">Permissions</span></span>

<span data-ttu-id="9fc9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fc9a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fc9a-109">Permission type</span></span>                        | <span data-ttu-id="9fc9a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fc9a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9fc9a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fc9a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fc9a-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9fc9a-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9fc9a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fc9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc9a-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9fc9a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="9fc9a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fc9a-115">Application</span></span>                            | <span data-ttu-id="9fc9a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc9a-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="9fc9a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc9a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="9fc9a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc9a-118">Request headers</span></span>

| <span data-ttu-id="9fc9a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9fc9a-119">Name</span></span>           |<span data-ttu-id="9fc9a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fc9a-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="9fc9a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fc9a-121">Authorization</span></span>  | <span data-ttu-id="9fc9a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9fc9a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9fc9a-124">Content-Type</span></span>   | <span data-ttu-id="9fc9a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fc9a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc9a-127">Request body</span></span>

<span data-ttu-id="9fc9a-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9fc9a-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9fc9a-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9fc9a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fc9a-131">Property</span></span>           | <span data-ttu-id="9fc9a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fc9a-132">Type</span></span>                                                                  | <span data-ttu-id="9fc9a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fc9a-133">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="9fc9a-134">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="9fc9a-134">completionMonthYear</span></span> |<span data-ttu-id="9fc9a-135">Data</span><span class="sxs-lookup"><span data-stu-id="9fc9a-135">Date</span></span>                                                                   | <span data-ttu-id="9fc9a-136">O mês e o ano em que o usuário formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-136">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="9fc9a-137">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="9fc9a-137">endMonthYear</span></span>        |<span data-ttu-id="9fc9a-138">Data</span><span class="sxs-lookup"><span data-stu-id="9fc9a-138">Date</span></span>                                                                   | <span data-ttu-id="9fc9a-139">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-139">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="9fc9a-140">instituição</span><span class="sxs-lookup"><span data-stu-id="9fc9a-140">institution</span></span>         |[<span data-ttu-id="9fc9a-141">institutionData</span><span class="sxs-lookup"><span data-stu-id="9fc9a-141">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="9fc9a-142">Contém detalhes da instituição estudada em.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-142">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="9fc9a-143">programa</span><span class="sxs-lookup"><span data-stu-id="9fc9a-143">program</span></span>             |[<span data-ttu-id="9fc9a-144">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="9fc9a-144">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="9fc9a-145">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-145">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="9fc9a-146">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="9fc9a-146">startMonthYear</span></span>      |<span data-ttu-id="9fc9a-147">Data</span><span class="sxs-lookup"><span data-stu-id="9fc9a-147">Date</span></span>                                                                   | <span data-ttu-id="9fc9a-148">O mês e o ano em que o usuário tiver iniciado a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-148">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="9fc9a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fc9a-149">Response</span></span>

<span data-ttu-id="9fc9a-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationalActivity](../resources/educationalactivity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-150">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fc9a-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9fc9a-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9fc9a-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc9a-152">Request</span></span>

<span data-ttu-id="9fc9a-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9fc9a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc9a-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9fc9a-155">C#</span><span class="sxs-lookup"><span data-stu-id="9fc9a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fc9a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fc9a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fc9a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fc9a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9fc9a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fc9a-158">Response</span></span>

<span data-ttu-id="9fc9a-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-159">The following is an example of the response.</span></span>

> <span data-ttu-id="9fc9a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fc9a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
