---
title: Listar recursos de tarefa
description: Obter todos os recursos associados a essa atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6d9363bb6127bde54cd7e56eae382fae621185d7
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912159"
---
# <a name="list-assignment-resources"></a><span data-ttu-id="4c91d-103">Listar recursos de tarefa</span><span class="sxs-lookup"><span data-stu-id="4c91d-103">List assignment resources</span></span>

<span data-ttu-id="4c91d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c91d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c91d-105">Obter todos os recursos associados a uma [atribuição](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4c91d-105">Get all the resources associated with an [assignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c91d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c91d-106">Permissions</span></span>
<span data-ttu-id="4c91d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c91d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c91d-109">Permission type</span></span>      | <span data-ttu-id="4c91d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c91d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c91d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c91d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c91d-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c91d-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4c91d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c91d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4c91d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c91d-114">Not supported.</span></span>  |
|<span data-ttu-id="4c91d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c91d-115">Application</span></span> | <span data-ttu-id="4c91d-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c91d-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c91d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c91d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c91d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c91d-118">Optional query parameters</span></span>
<span data-ttu-id="4c91d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c91d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c91d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c91d-120">Request headers</span></span>
| <span data-ttu-id="4c91d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c91d-121">Header</span></span>       | <span data-ttu-id="4c91d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c91d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c91d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c91d-123">Authorization</span></span>  | <span data-ttu-id="4c91d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c91d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c91d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c91d-126">Request body</span></span>
<span data-ttu-id="4c91d-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="4c91d-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c91d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c91d-128">Response</span></span>
<span data-ttu-id="4c91d-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c91d-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c91d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c91d-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c91d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c91d-131">Request</span></span>
<span data-ttu-id="4c91d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c91d-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/d38ffdea-da93-46ac-90ba-d568c6073075/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources
```

### <a name="response"></a><span data-ttu-id="4c91d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c91d-133">Response</span></span>
<span data-ttu-id="4c91d-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c91d-134">The following is an example of the response.</span></span> 

><span data-ttu-id="4c91d-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c91d-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
      "resource": {
          "@odata.type": "#microsoft.graph.educationWordResource",
          "displayName": "Report.docx",
          "createdDateTime": "2017-10-21T07:52:53.9863696Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
