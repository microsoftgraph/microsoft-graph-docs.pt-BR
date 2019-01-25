---
title: Criar um educationSynchronizationProfile
description: 'Crie uma solicitação para um novo perfil de sincronização de dados escola no inquilino. Consulte o status para obter o status do perfil. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: efc9b76405b57d0e47d645d0e7b00dc9425ba71b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520812"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="68fac-104">Criar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="68fac-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68fac-105">Crie uma solicitação para um novo escola dados [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="68fac-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="68fac-106">[O status da consulta](educationsynchronizationprofilestatus-get.md) para obter o status do perfil.</span><span class="sxs-lookup"><span data-stu-id="68fac-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="68fac-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="68fac-107">Permissions</span></span>
<span data-ttu-id="68fac-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68fac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68fac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68fac-110">Permission type</span></span> | <span data-ttu-id="68fac-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="68fac-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="68fac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68fac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68fac-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68fac-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="68fac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68fac-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="68fac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68fac-115">Not supported.</span></span>|
|<span data-ttu-id="68fac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68fac-116">Application</span></span>|<span data-ttu-id="68fac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68fac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68fac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68fac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="68fac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68fac-119">Request headers</span></span>
| <span data-ttu-id="68fac-120">Nome</span><span class="sxs-lookup"><span data-stu-id="68fac-120">Name</span></span>       | <span data-ttu-id="68fac-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="68fac-121">Type</span></span> | <span data-ttu-id="68fac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="68fac-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68fac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="68fac-123">Authorization</span></span>  | <span data-ttu-id="68fac-124">string</span><span class="sxs-lookup"><span data-stu-id="68fac-124">string</span></span>  | <span data-ttu-id="68fac-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68fac-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68fac-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68fac-127">Content-Type</span></span> | <span data-ttu-id="68fac-128">string</span><span class="sxs-lookup"><span data-stu-id="68fac-128">string</span></span> | <span data-ttu-id="68fac-129">application/json</span><span class="sxs-lookup"><span data-stu-id="68fac-129">Application/json.</span></span> <span data-ttu-id="68fac-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68fac-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68fac-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68fac-131">Request body</span></span>
<span data-ttu-id="68fac-132">No corpo da solicitação, fornece uma representação JSON do objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="68fac-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68fac-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="68fac-133">Response</span></span>
<span data-ttu-id="68fac-134">Se tiver êxito, este método retornará um `202, Accepted` código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68fac-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68fac-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68fac-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68fac-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68fac-136">Request</span></span>
<span data-ttu-id="68fac-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68fac-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="68fac-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="68fac-138">Response</span></span>
<span data-ttu-id="68fac-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68fac-139">The following is an example of the response.</span></span> 

><span data-ttu-id="68fac-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68fac-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
