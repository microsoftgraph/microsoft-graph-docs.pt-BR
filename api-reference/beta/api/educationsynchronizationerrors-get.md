---
title: Obter educationSynchronizationErrors
description: 'Obtenha os erros gerados durante a validação e/ou durante uma sincronização de um perfil de sincronização de dados escolar específico no locatário. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 31422cbc4b9a6badb637c23cd6f11b2471e342db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259469"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="f22d1-103">Obter educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="f22d1-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="f22d1-104">Obtenha os erros gerados durante a validação e/ou durante uma sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="f22d1-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f22d1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f22d1-105">Permissions</span></span>
<span data-ttu-id="f22d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f22d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f22d1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f22d1-108">Permission type</span></span> | <span data-ttu-id="f22d1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f22d1-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="f22d1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f22d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f22d1-111">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f22d1-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f22d1-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f22d1-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f22d1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f22d1-113">Not supported.</span></span>|
|<span data-ttu-id="f22d1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f22d1-114">Application</span></span>| <span data-ttu-id="f22d1-115">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f22d1-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f22d1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f22d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f22d1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f22d1-117">Optional query parameters</span></span>
<span data-ttu-id="f22d1-118">Este método dá suporte aos seguintes [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e $Count.</span><span class="sxs-lookup"><span data-stu-id="f22d1-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f22d1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f22d1-119">Request headers</span></span>
| <span data-ttu-id="f22d1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f22d1-120">Name</span></span>       | <span data-ttu-id="f22d1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f22d1-121">Type</span></span> | <span data-ttu-id="f22d1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f22d1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f22d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f22d1-123">Authorization</span></span>  | <span data-ttu-id="f22d1-124">string</span><span class="sxs-lookup"><span data-stu-id="f22d1-124">string</span></span>  | <span data-ttu-id="f22d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f22d1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f22d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f22d1-127">Request body</span></span>
<span data-ttu-id="f22d1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f22d1-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f22d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22d1-129">Response</span></span>
<span data-ttu-id="f22d1-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [erro de sincronização](../resources/educationsynchronizationerror.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f22d1-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f22d1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f22d1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f22d1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f22d1-132">Request</span></span>
<span data-ttu-id="f22d1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f22d1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```

##### <a name="response"></a><span data-ttu-id="f22d1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22d1-134">Response</span></span>
<span data-ttu-id="f22d1-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f22d1-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f22d1-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f22d1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f22d1-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f22d1-138">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f22d1-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f22d1-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_error-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="f22d1-140">C#</span><span class="sxs-lookup"><span data-stu-id="f22d1-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_error-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f22d1-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f22d1-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_error-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationerrors-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationerrors-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationerrors-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
