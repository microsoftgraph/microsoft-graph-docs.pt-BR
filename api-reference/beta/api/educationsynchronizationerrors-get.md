---
title: Obter educationSynchronizationErrors
description: 'Obter os erros gerados durante a validação e/ou durante uma sincronização de um perfil específico de sincronização de dados escolares no locatário. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a3b2e0b9018d3a6d34073530f8bd846a4d6df64c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574262"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="b65cc-103">Obter educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="b65cc-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="b65cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b65cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b65cc-105">Obter os erros gerados durante a validação e/ou durante uma sincronização de um perfil específico de sincronização de dados [escolares](../resources/educationsynchronizationprofile.md) no locatário.</span><span class="sxs-lookup"><span data-stu-id="b65cc-105">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b65cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b65cc-106">Permissions</span></span>

<span data-ttu-id="b65cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b65cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b65cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b65cc-109">Permission type</span></span>                       | <span data-ttu-id="b65cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b65cc-110">Permissions (from least to most privileged)</span></span>                 |
| :------------------------------------ | :---------------------------------------------------------- |
| <span data-ttu-id="b65cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b65cc-111">Delegated (work or school account)</span></span>    | <span data-ttu-id="b65cc-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b65cc-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span>         |
| <span data-ttu-id="b65cc-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b65cc-113">Delegated (personal Microsoft account</span></span> | <span data-ttu-id="b65cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b65cc-114">Not supported.</span></span>                                              |
| <span data-ttu-id="b65cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b65cc-115">Application</span></span>                           | <span data-ttu-id="b65cc-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b65cc-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b65cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b65cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/synchronizationProfiles/{id}/errors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b65cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b65cc-118">Optional query parameters</span></span>

<span data-ttu-id="b65cc-119">Este método dá suporte aos seguintes Parâmetros de Consulta [OData](/graph/query-parameters) para ajudar a personalizar a resposta: $filter, $orderby, $top, $skip e \$ contagem.</span><span class="sxs-lookup"><span data-stu-id="b65cc-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and \$count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b65cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b65cc-120">Request headers</span></span>

| <span data-ttu-id="b65cc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b65cc-121">Name</span></span>          | <span data-ttu-id="b65cc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b65cc-122">Type</span></span>   | <span data-ttu-id="b65cc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b65cc-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="b65cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b65cc-124">Authorization</span></span> | <span data-ttu-id="b65cc-125">string</span><span class="sxs-lookup"><span data-stu-id="b65cc-125">string</span></span> | <span data-ttu-id="b65cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b65cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b65cc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b65cc-128">Request body</span></span>

<span data-ttu-id="b65cc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b65cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b65cc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b65cc-130">Response</span></span>

<span data-ttu-id="b65cc-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos de erro de `200 OK` sincronização no corpo da resposta. [](../resources/educationsynchronizationerror.md)</span><span class="sxs-lookup"><span data-stu-id="b65cc-131">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b65cc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b65cc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b65cc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b65cc-133">Request</span></span>

<span data-ttu-id="b65cc-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b65cc-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b65cc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b65cc-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[<span data-ttu-id="b65cc-136">C#</span><span class="sxs-lookup"><span data-stu-id="b65cc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b65cc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b65cc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b65cc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b65cc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b65cc-139">Java</span><span class="sxs-lookup"><span data-stu-id="b65cc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b65cc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b65cc-140">Response</span></span>

<span data-ttu-id="b65cc-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b65cc-141">The following is an example of the response.</span></span>

> <span data-ttu-id="b65cc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b65cc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/errors",
  "@odata.count": 14,
  "value": [
    {
      "id": "92797B7C-02C3-4326-8ACC-E81C78753831",
      "entryType": "Student",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
      "joiningValue": "richard.2wilson@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:45Z",
      "reportableIdentifier": "richard.2wilson"
    },
    {
      "id": "94C1EB0E-8339-4EF4-8CB2-EB15C6228CE1",
      "entryType": "Teacher",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
      "joiningValue": "alberto2.dorsey@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:57Z",
      "reportableIdentifier": "alberto2.dorsey"
    },
    {
      "id": "98A82052-7716-49E9-90CC-C6FF406FC8E5",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
