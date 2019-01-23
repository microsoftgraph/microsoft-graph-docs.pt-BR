---
title: Lista educationSynchronizationProfiles
description: Recupere a coleção de perfis de sincronização de dados escola no inquilino.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ed001a7c265f16057ea216d21f7a05f672df7065
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425068"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="f9b18-103">Lista educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="f9b18-103">List educationSynchronizationProfiles</span></span>

> <span data-ttu-id="f9b18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9b18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9b18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9b18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9b18-106">Recupere a coleção de [perfis de sincronização](../resources/educationsynchronizationprofile.md) de dados escola no inquilino.</span><span class="sxs-lookup"><span data-stu-id="f9b18-106">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9b18-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9b18-107">Permissions</span></span>
<span data-ttu-id="f9b18-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9b18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9b18-110">Permission type</span></span> | <span data-ttu-id="f9b18-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9b18-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f9b18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9b18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9b18-113">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9b18-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f9b18-114">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f9b18-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f9b18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b18-115">Not supported.</span></span>|
|<span data-ttu-id="f9b18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9b18-116">Application</span></span>|<span data-ttu-id="f9b18-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9b18-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9b18-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9b18-119">Optional query parameters</span></span>
<span data-ttu-id="f9b18-120">Esse método suporta os seguintes [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip, Skip e $count.</span><span class="sxs-lookup"><span data-stu-id="f9b18-120">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9b18-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b18-121">Request headers</span></span>
| <span data-ttu-id="f9b18-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f9b18-122">Name</span></span>       | <span data-ttu-id="f9b18-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9b18-123">Type</span></span> | <span data-ttu-id="f9b18-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b18-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9b18-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9b18-125">Authorization</span></span>  | <span data-ttu-id="f9b18-126">string</span><span class="sxs-lookup"><span data-stu-id="f9b18-126">string</span></span>  | <span data-ttu-id="f9b18-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9b18-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9b18-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b18-129">Request body</span></span>
<span data-ttu-id="f9b18-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9b18-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f9b18-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b18-131">Response</span></span>
<span data-ttu-id="f9b18-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b18-132">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b18-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9b18-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9b18-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b18-134">Request</span></span>
<span data-ttu-id="f9b18-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9b18-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="f9b18-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b18-136">Response</span></span>
<span data-ttu-id="f9b18-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b18-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f9b18-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9b18-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
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
  ]
}
```
