---
title: Listar educationSynchronizationProfiles
description: Recupere a coleção de perfis de sincronização de dados escolares no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 707e8728ee5ef250ea33e88102cb534b399c3684
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043098"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="63754-103">Listar educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="63754-103">List educationSynchronizationProfiles</span></span>

<span data-ttu-id="63754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63754-105">Recupere a coleção de perfis de [sincronização de](../resources/educationsynchronizationprofile.md) dados escolares no locatário.</span><span class="sxs-lookup"><span data-stu-id="63754-105">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="63754-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63754-106">Permissions</span></span>
<span data-ttu-id="63754-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63754-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63754-109">Permission type</span></span> | <span data-ttu-id="63754-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63754-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="63754-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63754-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63754-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63754-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="63754-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="63754-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="63754-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63754-114">Not supported.</span></span>|
|<span data-ttu-id="63754-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63754-115">Application</span></span>|<span data-ttu-id="63754-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63754-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63754-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63754-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63754-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63754-118">Optional query parameters</span></span>
<span data-ttu-id="63754-119">Este método oferece suporte aos seguintes Parâmetros de Consulta [OData](/graph/query-parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e $count.</span><span class="sxs-lookup"><span data-stu-id="63754-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63754-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63754-120">Request headers</span></span>
| <span data-ttu-id="63754-121">Nome</span><span class="sxs-lookup"><span data-stu-id="63754-121">Name</span></span>       | <span data-ttu-id="63754-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="63754-122">Type</span></span> | <span data-ttu-id="63754-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="63754-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="63754-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="63754-124">Authorization</span></span>  | <span data-ttu-id="63754-125">string</span><span class="sxs-lookup"><span data-stu-id="63754-125">string</span></span>  | <span data-ttu-id="63754-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63754-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63754-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63754-128">Request body</span></span>
<span data-ttu-id="63754-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63754-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="63754-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="63754-130">Response</span></span>
<span data-ttu-id="63754-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63754-131">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63754-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63754-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63754-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63754-133">Request</span></span>
<span data-ttu-id="63754-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63754-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63754-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="63754-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_synchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```
# <a name="c"></a>[<span data-ttu-id="63754-136">C#</span><span class="sxs-lookup"><span data-stu-id="63754-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63754-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63754-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63754-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63754-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63754-139">Java</span><span class="sxs-lookup"><span data-stu-id="63754-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="63754-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="63754-140">Response</span></span>
<span data-ttu-id="63754-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63754-141">The following is an example of the response.</span></span> 

><span data-ttu-id="63754-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="63754-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "studentEnrollment": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacherRoster": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                }
            }
        },
        "identitySynchronizationConfiguration": {
            "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
            "userDomains": [
                {
                    "appliesTo": "student",
                    "name": "testschool.edu"
                },
                {
                    "appliesTo": "teacher",
                    "name": "testschool.edu"
                }
            ]
        },
        "licensesToAssign": [
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "student",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            }
        ]
    }
  ]
}
```
