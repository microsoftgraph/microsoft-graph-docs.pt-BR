---
title: Listar educationalActivities
description: Recupere uma lista de objetos educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ab8a9800bd6c8517fd4d3fc84b1485549c4ed4ba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037274"
---
# <a name="list-educationalactivities"></a><span data-ttu-id="75c90-103">Listar educationalActivities</span><span class="sxs-lookup"><span data-stu-id="75c90-103">List educationalActivities</span></span>

<span data-ttu-id="75c90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75c90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75c90-105">Recupere uma lista de [objetos educationalActivity](../resources/educationalactivity.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="75c90-105">Retrieve a list of [educationalActivity](../resources/educationalactivity.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="75c90-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="75c90-106">Permissions</span></span>

<span data-ttu-id="75c90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75c90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75c90-109">Permission type</span></span>                        | <span data-ttu-id="75c90-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75c90-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="75c90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75c90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75c90-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c90-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="75c90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75c90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75c90-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c90-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="75c90-115">Application</span><span class="sxs-lookup"><span data-stu-id="75c90-115">Application</span></span>                            | <span data-ttu-id="75c90-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c90-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="75c90-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75c90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities
GET /users/{id | userPrincipalName}/profile/educationalActivities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75c90-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="75c90-118">Optional query parameters</span></span>

<span data-ttu-id="75c90-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="75c90-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="75c90-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75c90-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="75c90-121">Nome</span><span class="sxs-lookup"><span data-stu-id="75c90-121">Name</span></span>            |<span data-ttu-id="75c90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75c90-122">Value</span></span>    |<span data-ttu-id="75c90-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="75c90-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="75c90-124">$filter</span><span class="sxs-lookup"><span data-stu-id="75c90-124">$filter</span></span>         |<span data-ttu-id="75c90-125">string</span><span class="sxs-lookup"><span data-stu-id="75c90-125">string</span></span>   |<span data-ttu-id="75c90-126">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="75c90-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="75c90-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="75c90-127">$orderby</span></span>        |<span data-ttu-id="75c90-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75c90-128">string</span></span>   |<span data-ttu-id="75c90-129">Por padrão, os objetos na resposta são classificação pelo valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="75c90-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="75c90-130">Você pode alterar a ordem da resposta usando o parâmetro *$orderby.*</span><span class="sxs-lookup"><span data-stu-id="75c90-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="75c90-131">$select</span><span class="sxs-lookup"><span data-stu-id="75c90-131">$select</span></span>         |<span data-ttu-id="75c90-132">string</span><span class="sxs-lookup"><span data-stu-id="75c90-132">string</span></span>   |<span data-ttu-id="75c90-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="75c90-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="75c90-135">$skip</span><span class="sxs-lookup"><span data-stu-id="75c90-135">$skip</span></span>           |<span data-ttu-id="75c90-136">int</span><span class="sxs-lookup"><span data-stu-id="75c90-136">int</span></span>      |<span data-ttu-id="75c90-137">Ignore os primeiros resultados n, úteis para pajamento.</span><span class="sxs-lookup"><span data-stu-id="75c90-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="75c90-138">$top</span><span class="sxs-lookup"><span data-stu-id="75c90-138">$top</span></span>            |<span data-ttu-id="75c90-139">int</span><span class="sxs-lookup"><span data-stu-id="75c90-139">int</span></span>      |<span data-ttu-id="75c90-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="75c90-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="75c90-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75c90-141">Request headers</span></span>

| <span data-ttu-id="75c90-142">Nome</span><span class="sxs-lookup"><span data-stu-id="75c90-142">Name</span></span>           |<span data-ttu-id="75c90-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="75c90-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="75c90-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="75c90-144">Authorization</span></span>  | <span data-ttu-id="75c90-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75c90-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="75c90-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75c90-147">Request body</span></span>

<span data-ttu-id="75c90-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75c90-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75c90-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="75c90-149">Response</span></span>

<span data-ttu-id="75c90-150">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [educationalActivity](../resources/educationalactivity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75c90-150">If successful, this method returns a `200 OK` response code and a collection of [educationalActivity](../resources/educationalactivity.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75c90-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="75c90-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75c90-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75c90-152">Request</span></span>

<span data-ttu-id="75c90-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="75c90-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75c90-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="75c90-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationalactivities"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities
```
# <a name="c"></a>[<span data-ttu-id="75c90-155">C#</span><span class="sxs-lookup"><span data-stu-id="75c90-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75c90-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75c90-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75c90-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75c90-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75c90-158">Java</span><span class="sxs-lookup"><span data-stu-id="75c90-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationalactivities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75c90-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="75c90-159">Response</span></span>

<span data-ttu-id="75c90-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="75c90-160">The following is an example of the response.</span></span>

> <span data-ttu-id="75c90-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="75c90-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```


