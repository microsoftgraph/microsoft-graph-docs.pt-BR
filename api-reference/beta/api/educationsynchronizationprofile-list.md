---
title: Listar educationSynchronizationProfiles
description: Recupere o conjunto de perfis de sincronização de dados da escola no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1907b0ef08473a79d66e79fcb4751b281e9a18ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457456"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="2e6dd-103">Listar educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="2e6dd-103">List educationSynchronizationProfiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e6dd-104">Recupere o conjunto de perfis de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-104">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e6dd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e6dd-105">Permissions</span></span>
<span data-ttu-id="2e6dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e6dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e6dd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e6dd-108">Permission type</span></span> | <span data-ttu-id="2e6dd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e6dd-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2e6dd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e6dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e6dd-111">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e6dd-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2e6dd-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2e6dd-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2e6dd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-113">Not supported.</span></span>|
|<span data-ttu-id="2e6dd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e6dd-114">Application</span></span>|<span data-ttu-id="2e6dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e6dd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e6dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e6dd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e6dd-117">Optional query parameters</span></span>
<span data-ttu-id="2e6dd-118">Este método dá suporte aos seguintes [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e $Count.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e6dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e6dd-119">Request headers</span></span>
| <span data-ttu-id="2e6dd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2e6dd-120">Name</span></span>       | <span data-ttu-id="2e6dd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e6dd-121">Type</span></span> | <span data-ttu-id="2e6dd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6dd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e6dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e6dd-123">Authorization</span></span>  | <span data-ttu-id="2e6dd-124">string</span><span class="sxs-lookup"><span data-stu-id="2e6dd-124">string</span></span>  | <span data-ttu-id="2e6dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e6dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e6dd-127">Request body</span></span>
<span data-ttu-id="2e6dd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2e6dd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e6dd-129">Response</span></span>
<span data-ttu-id="2e6dd-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-130">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e6dd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e6dd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e6dd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e6dd-132">Request</span></span>
<span data-ttu-id="2e6dd-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="2e6dd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e6dd-134">Response</span></span>
<span data-ttu-id="2e6dd-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2e6dd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e6dd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
