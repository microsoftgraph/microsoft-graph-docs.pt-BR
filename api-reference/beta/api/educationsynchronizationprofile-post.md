---
title: Criar um educationSynchronizationProfile
description: 'Crie uma solicitação para um novo perfil de sincronização de dados escolares no locatário. Consulte o status para obter o status do perfil. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e55a24642f6b29ce280775f779f005fd76d4996c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043070"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="f0c1a-104">Criar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="f0c1a-104">Create an educationSynchronizationProfile</span></span>

<span data-ttu-id="f0c1a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0c1a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c1a-106">Crie uma solicitação para um novo perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolares no locatário.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-106">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f0c1a-107">[Consulte o status para](educationsynchronizationprofilestatus-get.md) obter o status do perfil.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-107">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f0c1a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0c1a-108">Permissions</span></span>
<span data-ttu-id="f0c1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0c1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0c1a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0c1a-111">Permission type</span></span> | <span data-ttu-id="f0c1a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0c1a-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f0c1a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0c1a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f0c1a-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0c1a-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f0c1a-115">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f0c1a-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f0c1a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-116">Not supported.</span></span>|
|<span data-ttu-id="f0c1a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0c1a-117">Application</span></span>|<span data-ttu-id="f0c1a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0c1a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c1a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f0c1a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c1a-120">Request headers</span></span>
| <span data-ttu-id="f0c1a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f0c1a-121">Name</span></span>       | <span data-ttu-id="f0c1a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0c1a-122">Type</span></span> | <span data-ttu-id="f0c1a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c1a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0c1a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0c1a-124">Authorization</span></span>  | <span data-ttu-id="f0c1a-125">string</span><span class="sxs-lookup"><span data-stu-id="f0c1a-125">string</span></span>  | <span data-ttu-id="f0c1a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0c1a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0c1a-128">Content-Type</span></span> | <span data-ttu-id="f0c1a-129">string</span><span class="sxs-lookup"><span data-stu-id="f0c1a-129">string</span></span> | <span data-ttu-id="f0c1a-130">Application/json.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-130">Application/json.</span></span> <span data-ttu-id="f0c1a-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0c1a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c1a-132">Request body</span></span>
<span data-ttu-id="f0c1a-133">No corpo da solicitação, fornece uma representação JSON do [objeto educationSynchronizationProfile.](../resources/educationsynchronizationprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0c1a-133">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f0c1a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c1a-134">Response</span></span>
<span data-ttu-id="f0c1a-135">Se tiver êxito, este método retornará um código de resposta e um `202, Accepted` [objeto educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-135">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0c1a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0c1a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0c1a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c1a-137">Request</span></span>
<span data-ttu-id="f0c1a-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-138">The following is an example of the request.</span></span>
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
        "@odata.type": "#Microsoft.Education.DataSync.educationCsvDataProvider",
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
        "@odata.type": "#Microsoft.Education.DataSync.educationIdentityCreationConfiguration",
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

##### <a name="response"></a><span data-ttu-id="f0c1a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c1a-139">Response</span></span>
<span data-ttu-id="f0c1a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-140">The following is an example of the response.</span></span> 

><span data-ttu-id="f0c1a-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f0c1a-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
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


