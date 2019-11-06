---
title: Obter educationalActivity
description: Recupere as propriedades e os relacionamentos de um objeto educationalactivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 980f7f246ec40a8822502c3c22497ee408f2fe8c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994775"
---
# <a name="get-educationalactivity"></a><span data-ttu-id="7f80f-103">Obter educationalActivity</span><span class="sxs-lookup"><span data-stu-id="7f80f-103">Get educationalActivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f80f-104">Recupere as propriedades e os relacionamentos de um objeto [educationalActivity](../resources/educationalactivity.md) de um perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="7f80f-104">Retrieve the properties and relationships of an [educationalActivity](../resources/educationalactivity.md) object from a users profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f80f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f80f-105">Permissions</span></span>

<span data-ttu-id="7f80f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f80f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f80f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f80f-108">Permission type</span></span>                        | <span data-ttu-id="7f80f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f80f-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="7f80f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f80f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f80f-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7f80f-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7f80f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f80f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f80f-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7f80f-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7f80f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f80f-114">Application</span></span>                            | <span data-ttu-id="7f80f-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7f80f-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="7f80f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f80f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f80f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f80f-117">Optional query parameters</span></span>

<span data-ttu-id="7f80f-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f80f-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="7f80f-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7f80f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="7f80f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7f80f-120">Name</span></span>            |<span data-ttu-id="7f80f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7f80f-121">Value</span></span>    |<span data-ttu-id="7f80f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f80f-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7f80f-123">$filter</span><span class="sxs-lookup"><span data-stu-id="7f80f-123">$filter</span></span>         |<span data-ttu-id="7f80f-124">string</span><span class="sxs-lookup"><span data-stu-id="7f80f-124">string</span></span>   |<span data-ttu-id="7f80f-125">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="7f80f-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="7f80f-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="7f80f-126">$orderby</span></span>        |<span data-ttu-id="7f80f-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f80f-127">string</span></span>   |<span data-ttu-id="7f80f-128">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="7f80f-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="7f80f-129">Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7f80f-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="7f80f-130">$select</span><span class="sxs-lookup"><span data-stu-id="7f80f-130">$select</span></span>         |<span data-ttu-id="7f80f-131">string</span><span class="sxs-lookup"><span data-stu-id="7f80f-131">string</span></span>   |<span data-ttu-id="7f80f-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="7f80f-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="7f80f-134">$skip</span><span class="sxs-lookup"><span data-stu-id="7f80f-134">$skip</span></span>           |<span data-ttu-id="7f80f-135">int</span><span class="sxs-lookup"><span data-stu-id="7f80f-135">int</span></span>      |<span data-ttu-id="7f80f-136">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="7f80f-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="7f80f-137">$top</span><span class="sxs-lookup"><span data-stu-id="7f80f-137">$top</span></span>            |<span data-ttu-id="7f80f-138">int</span><span class="sxs-lookup"><span data-stu-id="7f80f-138">int</span></span>      |<span data-ttu-id="7f80f-139">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="7f80f-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="7f80f-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f80f-140">Request headers</span></span>

| <span data-ttu-id="7f80f-141">Nome</span><span class="sxs-lookup"><span data-stu-id="7f80f-141">Name</span></span>           |<span data-ttu-id="7f80f-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f80f-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7f80f-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f80f-143">Authorization</span></span>  | <span data-ttu-id="7f80f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f80f-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="7f80f-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f80f-146">Request body</span></span>

<span data-ttu-id="7f80f-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f80f-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f80f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f80f-148">Response</span></span>

<span data-ttu-id="7f80f-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [educationalActivity](../resources/educationalactivity.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f80f-149">If successful, this method returns a `200 OK` response code and the requested [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f80f-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7f80f-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f80f-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f80f-151">Request</span></span>

<span data-ttu-id="7f80f-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f80f-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f80f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f80f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationalactivity"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f80f-154">C#</span><span class="sxs-lookup"><span data-stu-id="7f80f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f80f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f80f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f80f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f80f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f80f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f80f-157">Response</span></span>

<span data-ttu-id="7f80f-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f80f-158">The following is an example of the response.</span></span>

> <span data-ttu-id="7f80f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f80f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
