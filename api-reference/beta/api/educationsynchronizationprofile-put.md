---
title: Atualizar um educationSynchronizationProfile
description: Atualize as propriedades de um perfil de sincronização de dados escola existente no inquilino.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0c99984b4ca0d8d72fdc02d28a8de80761fdbd60
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398734"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="90f1a-103">Atualizar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="90f1a-103">Update an educationSynchronizationProfile</span></span>

> <span data-ttu-id="90f1a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90f1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90f1a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90f1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90f1a-106">Atualize as propriedades de um existente escola dados do [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="90f1a-106">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="90f1a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90f1a-107">Permissions</span></span>
<span data-ttu-id="90f1a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90f1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90f1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90f1a-110">Permission type</span></span> | <span data-ttu-id="90f1a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="90f1a-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="90f1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90f1a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90f1a-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90f1a-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="90f1a-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="90f1a-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="90f1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90f1a-115">Not supported.</span></span>|
|<span data-ttu-id="90f1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90f1a-116">Application</span></span>|<span data-ttu-id="90f1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90f1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90f1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90f1a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="90f1a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90f1a-119">Request headers</span></span>
| <span data-ttu-id="90f1a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90f1a-120">Name</span></span>       | <span data-ttu-id="90f1a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="90f1a-121">Type</span></span> | <span data-ttu-id="90f1a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="90f1a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="90f1a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90f1a-123">Authorization</span></span>  | <span data-ttu-id="90f1a-124">string</span><span class="sxs-lookup"><span data-stu-id="90f1a-124">string</span></span>  | <span data-ttu-id="90f1a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90f1a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90f1a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90f1a-127">Content-Type</span></span> | <span data-ttu-id="90f1a-128">string</span><span class="sxs-lookup"><span data-stu-id="90f1a-128">string</span></span> | <span data-ttu-id="90f1a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90f1a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90f1a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90f1a-131">Request body</span></span>
<span data-ttu-id="90f1a-132">No corpo da solicitação, fornece uma representação JSON do objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="90f1a-132">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="90f1a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90f1a-133">Response</span></span>
<span data-ttu-id="90f1a-134">Se tiver êxito, este método retornará um `202, Accepted` código de resposta e um objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90f1a-134">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90f1a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90f1a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90f1a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90f1a-136">Request</span></span>
<span data-ttu-id="90f1a-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90f1a-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="90f1a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="90f1a-138">Response</span></span>
<span data-ttu-id="90f1a-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90f1a-139">Here is an example of the response.</span></span> 

><span data-ttu-id="90f1a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90f1a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
