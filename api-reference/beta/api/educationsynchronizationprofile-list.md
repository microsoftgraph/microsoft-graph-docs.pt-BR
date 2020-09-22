---
title: Listar educationSynchronizationProfiles
description: Recupere o conjunto de perfis de sincronização de dados da escola no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ac941da5ee0f5aafb5cbbfb59e58a7eba8f72d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007221"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="1358b-103">Listar educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="1358b-103">List educationSynchronizationProfiles</span></span>

<span data-ttu-id="1358b-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1358b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1358b-105">Recupere o conjunto de perfis de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário.</span><span class="sxs-lookup"><span data-stu-id="1358b-105">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1358b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1358b-106">Permissions</span></span>
<span data-ttu-id="1358b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1358b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1358b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1358b-109">Permission type</span></span> | <span data-ttu-id="1358b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1358b-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="1358b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1358b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1358b-112">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1358b-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1358b-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1358b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1358b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1358b-114">Not supported.</span></span>|
|<span data-ttu-id="1358b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1358b-115">Application</span></span>|<span data-ttu-id="1358b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1358b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1358b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1358b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1358b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1358b-118">Optional query parameters</span></span>
<span data-ttu-id="1358b-119">Este método dá suporte aos seguintes [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e $Count.</span><span class="sxs-lookup"><span data-stu-id="1358b-119">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1358b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1358b-120">Request headers</span></span>
| <span data-ttu-id="1358b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1358b-121">Name</span></span>       | <span data-ttu-id="1358b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1358b-122">Type</span></span> | <span data-ttu-id="1358b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1358b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1358b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1358b-124">Authorization</span></span>  | <span data-ttu-id="1358b-125">string</span><span class="sxs-lookup"><span data-stu-id="1358b-125">string</span></span>  | <span data-ttu-id="1358b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1358b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1358b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1358b-128">Request body</span></span>
<span data-ttu-id="1358b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1358b-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1358b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1358b-130">Response</span></span>
<span data-ttu-id="1358b-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1358b-131">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1358b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1358b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1358b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1358b-133">Request</span></span>
<span data-ttu-id="1358b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1358b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="1358b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1358b-135">Response</span></span>
<span data-ttu-id="1358b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1358b-136">The following is an example of the response.</span></span> 

><span data-ttu-id="1358b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1358b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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


