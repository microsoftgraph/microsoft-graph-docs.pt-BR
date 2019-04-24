---
title: Atualizar um educationSynchronizationProfile
description: Atualize as propriedades de um perfil de sincronização de dados da escola existente no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 668aad65abe2c9b3d4609400118f9341748210f1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464711"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="1c837-103">Atualizar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="1c837-103">Update an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c837-104">Atualize as propriedades de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola existente no locatário.</span><span class="sxs-lookup"><span data-stu-id="1c837-104">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c837-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c837-105">Permissions</span></span>
<span data-ttu-id="1c837-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c837-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c837-108">Permission type</span></span> | <span data-ttu-id="1c837-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c837-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="1c837-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c837-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c837-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c837-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1c837-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1c837-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1c837-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c837-113">Not supported.</span></span>|
|<span data-ttu-id="1c837-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c837-114">Application</span></span>|<span data-ttu-id="1c837-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c837-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c837-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c837-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1c837-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c837-117">Request headers</span></span>
| <span data-ttu-id="1c837-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1c837-118">Name</span></span>       | <span data-ttu-id="1c837-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c837-119">Type</span></span> | <span data-ttu-id="1c837-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c837-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c837-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c837-121">Authorization</span></span>  | <span data-ttu-id="1c837-122">string</span><span class="sxs-lookup"><span data-stu-id="1c837-122">string</span></span>  | <span data-ttu-id="1c837-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c837-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1c837-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c837-125">Content-Type</span></span> | <span data-ttu-id="1c837-126">string</span><span class="sxs-lookup"><span data-stu-id="1c837-126">string</span></span> | <span data-ttu-id="1c837-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c837-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c837-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c837-129">Request body</span></span>
<span data-ttu-id="1c837-130">No corpo da solicitação, forneça uma representação JSON do objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1c837-130">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1c837-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c837-131">Response</span></span>
<span data-ttu-id="1c837-132">Se tiver êxito, este método retornará `202, Accepted` um código de resposta e um objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c837-132">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c837-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c837-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c837-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c837-134">Request</span></span>
<span data-ttu-id="1c837-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c837-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_synchronizationProfile"
}-->
```http
PUT https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationcsvdataprovider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ]
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationidentitycreationconfiguration",
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
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="1c837-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c837-136">Response</span></span>
<span data-ttu-id="1c837-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c837-137">Here is an example of the response.</span></span> 

><span data-ttu-id="1c837-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c837-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
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
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
