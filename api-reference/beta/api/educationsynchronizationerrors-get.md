---
title: Obter educationSynchronizationErrors
description: 'Obtenha os erros gerados durante a validação e/ou durante uma sincronização de um perfil de sincronização de dados escolar específico no locatário. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 81da0a081976e97254b541c0d4d07e13ed51c854
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424607"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="99da0-103">Obter educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="99da0-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="99da0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="99da0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99da0-105">Obtenha os erros gerados durante a validação e/ou durante uma sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="99da0-105">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="99da0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="99da0-106">Permissions</span></span>
<span data-ttu-id="99da0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99da0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99da0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99da0-109">Permission type</span></span> | <span data-ttu-id="99da0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99da0-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="99da0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99da0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99da0-112">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99da0-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="99da0-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="99da0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="99da0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99da0-114">Not supported.</span></span>|
|<span data-ttu-id="99da0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99da0-115">Application</span></span>| <span data-ttu-id="99da0-116">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="99da0-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99da0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99da0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99da0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99da0-118">Optional query parameters</span></span>
<span data-ttu-id="99da0-119">Este método dá suporte aos seguintes [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e $Count.</span><span class="sxs-lookup"><span data-stu-id="99da0-119">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99da0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99da0-120">Request headers</span></span>
| <span data-ttu-id="99da0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="99da0-121">Name</span></span>       | <span data-ttu-id="99da0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="99da0-122">Type</span></span> | <span data-ttu-id="99da0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="99da0-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99da0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="99da0-124">Authorization</span></span>  | <span data-ttu-id="99da0-125">string</span><span class="sxs-lookup"><span data-stu-id="99da0-125">string</span></span>  | <span data-ttu-id="99da0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99da0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99da0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99da0-128">Request body</span></span>
<span data-ttu-id="99da0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99da0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="99da0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="99da0-130">Response</span></span>
<span data-ttu-id="99da0-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [erro de sincronização](../resources/educationsynchronizationerror.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99da0-131">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99da0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99da0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99da0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99da0-133">Request</span></span>
<span data-ttu-id="99da0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="99da0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99da0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="99da0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[<span data-ttu-id="99da0-136">C#</span><span class="sxs-lookup"><span data-stu-id="99da0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99da0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99da0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99da0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99da0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99da0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="99da0-139">Response</span></span>
<span data-ttu-id="99da0-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99da0-140">The following is an example of the response.</span></span> 

><span data-ttu-id="99da0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99da0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/errors",
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
