---
title: Obter um educationSynchronizationProfile
description: Recupere um perfil de sincronização de dados da escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52d40288237b417138d7ad54a290fc4529f3e10f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954855"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="fa137-103">Obter um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="fa137-103">Get an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa137-104">Recupere um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="fa137-104">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa137-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa137-105">Permissions</span></span>
<span data-ttu-id="fa137-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa137-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa137-108">Permission type</span></span> | <span data-ttu-id="fa137-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa137-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="fa137-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa137-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa137-111">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa137-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="fa137-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="fa137-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fa137-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa137-113">Not supported.</span></span>|
|<span data-ttu-id="fa137-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa137-114">Application</span></span>| <span data-ttu-id="fa137-115">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa137-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa137-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa137-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa137-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa137-117">Request headers</span></span>
| <span data-ttu-id="fa137-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fa137-118">Name</span></span>       | <span data-ttu-id="fa137-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa137-119">Type</span></span> | <span data-ttu-id="fa137-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa137-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fa137-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa137-121">Authorization</span></span>  | <span data-ttu-id="fa137-122">string</span><span class="sxs-lookup"><span data-stu-id="fa137-122">string</span></span>  | <span data-ttu-id="fa137-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa137-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa137-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa137-125">Request body</span></span>
<span data-ttu-id="fa137-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa137-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa137-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa137-127">Response</span></span>
<span data-ttu-id="fa137-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa137-128">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa137-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa137-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa137-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa137-130">Request</span></span>
<span data-ttu-id="fa137-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa137-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="fa137-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa137-132">Response</span></span>
<span data-ttu-id="fa137-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa137-133">The following is an example of the response.</span></span> 

><span data-ttu-id="fa137-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa137-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
