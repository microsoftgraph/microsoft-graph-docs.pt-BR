---
title: Obtenha um educationSynchronizationProfile
description: Recupere um perfil de sincronização de dados escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0c4d06583b7ba892cf2ae4bddd8de16cd8612082
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406329"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="c09de-103">Obtenha um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="c09de-103">Get an educationSynchronizationProfile</span></span>

> <span data-ttu-id="c09de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c09de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c09de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c09de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c09de-106">Recupere um de dados escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="c09de-106">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="c09de-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c09de-107">Permissions</span></span>
<span data-ttu-id="c09de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c09de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c09de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c09de-110">Permission type</span></span> | <span data-ttu-id="c09de-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c09de-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c09de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c09de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c09de-113">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c09de-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c09de-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c09de-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c09de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c09de-115">Not supported.</span></span>|
|<span data-ttu-id="c09de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c09de-116">Application</span></span>| <span data-ttu-id="c09de-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c09de-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c09de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c09de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c09de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c09de-119">Request headers</span></span>
| <span data-ttu-id="c09de-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c09de-120">Name</span></span>       | <span data-ttu-id="c09de-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c09de-121">Type</span></span> | <span data-ttu-id="c09de-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c09de-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c09de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c09de-123">Authorization</span></span>  | <span data-ttu-id="c09de-124">string</span><span class="sxs-lookup"><span data-stu-id="c09de-124">string</span></span>  | <span data-ttu-id="c09de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c09de-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c09de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c09de-127">Request body</span></span>
<span data-ttu-id="c09de-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c09de-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c09de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c09de-129">Response</span></span>
<span data-ttu-id="c09de-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c09de-130">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c09de-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c09de-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c09de-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c09de-132">Request</span></span>
<span data-ttu-id="c09de-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c09de-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="c09de-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c09de-134">Response</span></span>
<span data-ttu-id="c09de-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c09de-135">The following is an example of the response.</span></span> 

><span data-ttu-id="c09de-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c09de-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
