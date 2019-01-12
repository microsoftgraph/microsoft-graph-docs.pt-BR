---
title: Criar um educationSynchronizationProfile
description: 'Crie uma solicitação para um novo perfil de sincronização de dados escola no inquilino. Consulte o status para obter o status do perfil. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9d471766a8492e03809d05d6d0366c8e44d59015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915757"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="404d4-104">Criar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="404d4-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="404d4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="404d4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="404d4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="404d4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="404d4-107">Crie uma solicitação para um novo escola dados [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="404d4-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="404d4-108">[O status da consulta](educationsynchronizationprofilestatus-get.md) para obter o status do perfil.</span><span class="sxs-lookup"><span data-stu-id="404d4-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="404d4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="404d4-109">Permissions</span></span>
<span data-ttu-id="404d4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="404d4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="404d4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="404d4-112">Permission type</span></span> | <span data-ttu-id="404d4-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="404d4-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="404d4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="404d4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="404d4-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="404d4-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="404d4-116">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="404d4-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="404d4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="404d4-117">Not supported.</span></span>|
|<span data-ttu-id="404d4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="404d4-118">Application</span></span>|<span data-ttu-id="404d4-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="404d4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="404d4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="404d4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="404d4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="404d4-121">Request headers</span></span>
| <span data-ttu-id="404d4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="404d4-122">Name</span></span>       | <span data-ttu-id="404d4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="404d4-123">Type</span></span> | <span data-ttu-id="404d4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="404d4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="404d4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="404d4-125">Authorization</span></span>  | <span data-ttu-id="404d4-126">string</span><span class="sxs-lookup"><span data-stu-id="404d4-126">string</span></span>  | <span data-ttu-id="404d4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="404d4-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="404d4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="404d4-129">Content-Type</span></span> | <span data-ttu-id="404d4-130">string</span><span class="sxs-lookup"><span data-stu-id="404d4-130">string</span></span> | <span data-ttu-id="404d4-131">Aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="404d4-131">Application/json.</span></span> <span data-ttu-id="404d4-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="404d4-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="404d4-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="404d4-133">Request body</span></span>
<span data-ttu-id="404d4-134">No corpo da solicitação, fornece uma representação JSON do objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="404d4-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="404d4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="404d4-135">Response</span></span>
<span data-ttu-id="404d4-136">Se tiver êxito, este método retornará um `202, Accepted` código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="404d4-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="404d4-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="404d4-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="404d4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="404d4-138">Request</span></span>
<span data-ttu-id="404d4-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="404d4-139">The following is an example of the request.</span></span>
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
        "@odata.type": "#microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "#microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="404d4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="404d4-140">Response</span></span>
<span data-ttu-id="404d4-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="404d4-141">The following is an example of the response.</span></span> 

><span data-ttu-id="404d4-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="404d4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
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
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```
