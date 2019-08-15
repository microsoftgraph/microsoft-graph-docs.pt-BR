---
title: Obter educationSynchronizationErrors
description: 'Obtenha os erros gerados durante a validação e/ou durante uma sincronização de um perfil de sincronização de dados escolar específico no locatário. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a4b536d8021153c78bd2bc67fb943d2361b63215
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416020"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="b5157-103">Obter educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="b5157-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="b5157-104">Obtenha os erros gerados durante a validação e/ou durante uma sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="b5157-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b5157-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5157-105">Permissions</span></span>
<span data-ttu-id="b5157-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5157-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5157-108">Permission type</span></span> | <span data-ttu-id="b5157-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5157-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="b5157-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5157-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5157-111">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5157-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="b5157-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b5157-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b5157-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5157-113">Not supported.</span></span>|
|<span data-ttu-id="b5157-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5157-114">Application</span></span>| <span data-ttu-id="b5157-115">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b5157-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5157-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5157-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5157-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5157-117">Optional query parameters</span></span>
<span data-ttu-id="b5157-118">Este método dá suporte aos seguintes [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e $Count.</span><span class="sxs-lookup"><span data-stu-id="b5157-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5157-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5157-119">Request headers</span></span>
| <span data-ttu-id="b5157-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b5157-120">Name</span></span>       | <span data-ttu-id="b5157-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5157-121">Type</span></span> | <span data-ttu-id="b5157-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5157-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b5157-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5157-123">Authorization</span></span>  | <span data-ttu-id="b5157-124">string</span><span class="sxs-lookup"><span data-stu-id="b5157-124">string</span></span>  | <span data-ttu-id="b5157-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5157-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5157-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5157-127">Request body</span></span>
<span data-ttu-id="b5157-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5157-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b5157-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5157-129">Response</span></span>
<span data-ttu-id="b5157-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [erro de sincronização](../resources/educationsynchronizationerror.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5157-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5157-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5157-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5157-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5157-132">Request</span></span>
<span data-ttu-id="b5157-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5157-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b5157-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5157-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5157-135">C#</span><span class="sxs-lookup"><span data-stu-id="b5157-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5157-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5157-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5157-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b5157-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5157-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5157-138">Response</span></span>
<span data-ttu-id="b5157-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5157-139">The following is an example of the response.</span></span> 

><span data-ttu-id="b5157-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5157-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
