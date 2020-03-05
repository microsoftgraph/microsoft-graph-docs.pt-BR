---
title: Obter um educationSynchronizationProfile
description: Recupere um perfil de sincronização de dados da escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6c294ab025c148d851ee679c8b64c69608a470f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424481"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="38a11-103">Obter um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="38a11-103">Get an educationSynchronizationProfile</span></span>

<span data-ttu-id="38a11-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="38a11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a11-105">Recupere um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="38a11-105">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="38a11-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38a11-106">Permissions</span></span>
<span data-ttu-id="38a11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38a11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38a11-109">Permission type</span></span> | <span data-ttu-id="38a11-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38a11-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="38a11-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38a11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38a11-112">EduAdministration. Read, EduAdministration. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38a11-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="38a11-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="38a11-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="38a11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38a11-114">Not supported.</span></span>|
|<span data-ttu-id="38a11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38a11-115">Application</span></span>| <span data-ttu-id="38a11-116">EduAdministration. Read. All, EduAdministration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="38a11-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38a11-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38a11-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38a11-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38a11-118">Request headers</span></span>
| <span data-ttu-id="38a11-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38a11-119">Name</span></span>       | <span data-ttu-id="38a11-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="38a11-120">Type</span></span> | <span data-ttu-id="38a11-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a11-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38a11-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38a11-122">Authorization</span></span>  | <span data-ttu-id="38a11-123">string</span><span class="sxs-lookup"><span data-stu-id="38a11-123">string</span></span>  | <span data-ttu-id="38a11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38a11-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38a11-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38a11-126">Request body</span></span>
<span data-ttu-id="38a11-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38a11-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="38a11-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a11-128">Response</span></span>
<span data-ttu-id="38a11-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38a11-129">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38a11-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38a11-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38a11-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38a11-131">Request</span></span>
<span data-ttu-id="38a11-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38a11-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="38a11-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38a11-133">Response</span></span>
<span data-ttu-id="38a11-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38a11-134">The following is an example of the response.</span></span> 

><span data-ttu-id="38a11-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38a11-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
