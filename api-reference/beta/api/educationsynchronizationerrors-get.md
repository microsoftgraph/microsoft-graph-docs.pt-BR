---
title: Obter educationSynchronizationErrors
description: 'Obtenha os erros gerados durante a validação de e/ou durante uma sincronização de um perfil de sincronização de dados escola específico no inquilino. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a15070b68e9cf249a6b6a7841ea24b0e265a24e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926138"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="795eb-103">Obter educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="795eb-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="795eb-104">Obtenha os erros gerados durante a validação de e/ou durante uma sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="795eb-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="795eb-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="795eb-105">Permissions</span></span>
<span data-ttu-id="795eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="795eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="795eb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="795eb-108">Permission type</span></span> | <span data-ttu-id="795eb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="795eb-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="795eb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="795eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="795eb-111">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="795eb-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="795eb-112">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="795eb-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="795eb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="795eb-113">Not supported.</span></span>|
|<span data-ttu-id="795eb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="795eb-114">Application</span></span>| <span data-ttu-id="795eb-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="795eb-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="795eb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="795eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="795eb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="795eb-117">Optional query parameters</span></span>
<span data-ttu-id="795eb-118">Esse método suporta os seguintes [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip, Skip e $count.</span><span class="sxs-lookup"><span data-stu-id="795eb-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="795eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="795eb-119">Request headers</span></span>
| <span data-ttu-id="795eb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="795eb-120">Name</span></span>       | <span data-ttu-id="795eb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="795eb-121">Type</span></span> | <span data-ttu-id="795eb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="795eb-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="795eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="795eb-123">Authorization</span></span>  | <span data-ttu-id="795eb-124">string</span><span class="sxs-lookup"><span data-stu-id="795eb-124">string</span></span>  | <span data-ttu-id="795eb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="795eb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="795eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="795eb-127">Request body</span></span>
<span data-ttu-id="795eb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="795eb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="795eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="795eb-129">Response</span></span>
<span data-ttu-id="795eb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [erro de sincronização](../resources/educationsynchronizationerror.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="795eb-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="795eb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="795eb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="795eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="795eb-132">Request</span></span>
<span data-ttu-id="795eb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="795eb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```

##### <a name="response"></a><span data-ttu-id="795eb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="795eb-134">Response</span></span>
<span data-ttu-id="795eb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="795eb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="795eb-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="795eb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
