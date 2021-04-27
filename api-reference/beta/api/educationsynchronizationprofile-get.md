---
title: Obter um educationSynchronizationProfile
description: Recupere um perfil de sincronização de dados escolares no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1810fe299b62a52c2b56d9fccb2f312638beff06
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043105"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="e14d0-103">Obter um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e14d0-103">Get an educationSynchronizationProfile</span></span>

<span data-ttu-id="e14d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e14d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e14d0-105">Recupere um perfil de [sincronização de dados escolares](../resources/educationsynchronizationprofile.md) no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="e14d0-105">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="e14d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e14d0-106">Permissions</span></span>
<span data-ttu-id="e14d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e14d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e14d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e14d0-109">Permission type</span></span> | <span data-ttu-id="e14d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e14d0-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e14d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e14d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e14d0-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e14d0-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e14d0-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e14d0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e14d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e14d0-114">Not supported.</span></span>|
|<span data-ttu-id="e14d0-115">Application</span><span class="sxs-lookup"><span data-stu-id="e14d0-115">Application</span></span>| <span data-ttu-id="e14d0-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e14d0-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e14d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e14d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e14d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e14d0-118">Request headers</span></span>
| <span data-ttu-id="e14d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e14d0-119">Name</span></span>       | <span data-ttu-id="e14d0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e14d0-120">Type</span></span> | <span data-ttu-id="e14d0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e14d0-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e14d0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e14d0-122">Authorization</span></span>  | <span data-ttu-id="e14d0-123">string</span><span class="sxs-lookup"><span data-stu-id="e14d0-123">string</span></span>  | <span data-ttu-id="e14d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e14d0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e14d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e14d0-126">Request body</span></span>
<span data-ttu-id="e14d0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e14d0-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e14d0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e14d0-128">Response</span></span>
<span data-ttu-id="e14d0-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e14d0-129">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e14d0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e14d0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e14d0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e14d0-131">Request</span></span>
<span data-ttu-id="e14d0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e14d0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e14d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e14d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="e14d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="e14d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e14d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e14d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e14d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e14d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e14d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="e14d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e14d0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e14d0-138">Response</span></span>
<span data-ttu-id="e14d0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e14d0-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e14d0-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e14d0-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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


