---
title: Criar um educationSynchronizationProfile
description: 'Criar uma solicitação para um novo perfil de sincronização de dados da escola no locatário. Consultar o status para obter o status do perfil. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: efc9b76405b57d0e47d645d0e7b00dc9425ba71b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457400"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="db970-104">Criar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="db970-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db970-105">Criar uma solicitação para um novo perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário.</span><span class="sxs-lookup"><span data-stu-id="db970-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="db970-106">[Consultar o status](educationsynchronizationprofilestatus-get.md) para obter o status do perfil.</span><span class="sxs-lookup"><span data-stu-id="db970-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="db970-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="db970-107">Permissions</span></span>
<span data-ttu-id="db970-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db970-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db970-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db970-110">Permission type</span></span> | <span data-ttu-id="db970-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="db970-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="db970-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db970-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db970-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db970-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="db970-114">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="db970-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="db970-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db970-115">Not supported.</span></span>|
|<span data-ttu-id="db970-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db970-116">Application</span></span>|<span data-ttu-id="db970-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db970-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db970-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db970-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="db970-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db970-119">Request headers</span></span>
| <span data-ttu-id="db970-120">Nome</span><span class="sxs-lookup"><span data-stu-id="db970-120">Name</span></span>       | <span data-ttu-id="db970-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="db970-121">Type</span></span> | <span data-ttu-id="db970-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="db970-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db970-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db970-123">Authorization</span></span>  | <span data-ttu-id="db970-124">string</span><span class="sxs-lookup"><span data-stu-id="db970-124">string</span></span>  | <span data-ttu-id="db970-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db970-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="db970-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db970-127">Content-Type</span></span> | <span data-ttu-id="db970-128">string</span><span class="sxs-lookup"><span data-stu-id="db970-128">string</span></span> | <span data-ttu-id="db970-129">Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="db970-129">Application/json.</span></span> <span data-ttu-id="db970-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db970-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db970-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db970-131">Request body</span></span>
<span data-ttu-id="db970-132">No corpo da solicitação, forneça uma representação JSON do objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="db970-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db970-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="db970-133">Response</span></span>
<span data-ttu-id="db970-134">Se tiver êxito, este método retornará `202, Accepted` um código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db970-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db970-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db970-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db970-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db970-136">Request</span></span>
<span data-ttu-id="db970-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db970-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationSynchronizationProfile"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration",
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

##### <a name="response"></a><span data-ttu-id="db970-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="db970-138">Response</span></span>
<span data-ttu-id="db970-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db970-139">The following is an example of the response.</span></span> 

><span data-ttu-id="db970-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db970-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
