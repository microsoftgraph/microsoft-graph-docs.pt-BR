---
title: Atualizar um educationSynchronizationProfile
description: Atualize as propriedades de um perfil de sincronização de dados da escola existente no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2145db383d919b218a6d86115dba79d9b9e9875b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007081"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="d7607-103">Atualizar um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="d7607-103">Update an educationSynchronizationProfile</span></span>

<span data-ttu-id="d7607-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7607-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7607-105">Atualize as propriedades de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola existente no locatário.</span><span class="sxs-lookup"><span data-stu-id="d7607-105">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7607-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7607-106">Permissions</span></span>
<span data-ttu-id="d7607-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7607-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7607-109">Permission type</span></span> | <span data-ttu-id="d7607-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7607-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d7607-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7607-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7607-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7607-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="d7607-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d7607-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d7607-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7607-114">Not supported.</span></span>|
|<span data-ttu-id="d7607-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7607-115">Application</span></span>|<span data-ttu-id="d7607-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7607-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7607-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7607-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d7607-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7607-118">Request headers</span></span>
| <span data-ttu-id="d7607-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d7607-119">Name</span></span>       | <span data-ttu-id="d7607-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7607-120">Type</span></span> | <span data-ttu-id="d7607-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7607-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7607-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7607-122">Authorization</span></span>  | <span data-ttu-id="d7607-123">string</span><span class="sxs-lookup"><span data-stu-id="d7607-123">string</span></span>  | <span data-ttu-id="d7607-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7607-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7607-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7607-126">Content-Type</span></span> | <span data-ttu-id="d7607-127">string</span><span class="sxs-lookup"><span data-stu-id="d7607-127">string</span></span> | <span data-ttu-id="d7607-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7607-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7607-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7607-130">Request body</span></span>
<span data-ttu-id="d7607-131">No corpo da solicitação, forneça uma representação JSON do objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d7607-131">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7607-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7607-132">Response</span></span>
<span data-ttu-id="d7607-133">Se tiver êxito, este método retornará um `202, Accepted` código de resposta e um objeto [synchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7607-133">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7607-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7607-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7607-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7607-135">Request</span></span>
<span data-ttu-id="d7607-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7607-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d7607-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7607-137">Response</span></span>
<span data-ttu-id="d7607-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7607-138">Here is an example of the response.</span></span> 

><span data-ttu-id="d7607-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7607-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


