---
title: Obtenha um educationSynchronizationProfile
description: Recupere um perfil de sincronização de dados escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47757956db9e93bb13f4167ef330c7b79d7851b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530178"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="2b3bc-103">Obtenha um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="2b3bc-103">Get an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b3bc-104">Recupere um de dados escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-104">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b3bc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b3bc-105">Permissions</span></span>
<span data-ttu-id="2b3bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b3bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b3bc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b3bc-108">Permission type</span></span> | <span data-ttu-id="2b3bc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b3bc-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2b3bc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b3bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b3bc-111">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b3bc-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2b3bc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b3bc-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2b3bc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-113">Not supported.</span></span>|
|<span data-ttu-id="2b3bc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b3bc-114">Application</span></span>| <span data-ttu-id="2b3bc-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b3bc-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b3bc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b3bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b3bc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b3bc-117">Request headers</span></span>
| <span data-ttu-id="2b3bc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2b3bc-118">Name</span></span>       | <span data-ttu-id="2b3bc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b3bc-119">Type</span></span> | <span data-ttu-id="2b3bc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b3bc-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b3bc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b3bc-121">Authorization</span></span>  | <span data-ttu-id="2b3bc-122">string</span><span class="sxs-lookup"><span data-stu-id="2b3bc-122">string</span></span>  | <span data-ttu-id="2b3bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b3bc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b3bc-125">Request body</span></span>
<span data-ttu-id="2b3bc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2b3bc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b3bc-127">Response</span></span>
<span data-ttu-id="2b3bc-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-128">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b3bc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b3bc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b3bc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b3bc-130">Request</span></span>
<span data-ttu-id="2b3bc-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="2b3bc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b3bc-132">Response</span></span>
<span data-ttu-id="2b3bc-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-133">The following is an example of the response.</span></span> 

><span data-ttu-id="2b3bc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b3bc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
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
    "licensesToAssign": 
         [
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
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
