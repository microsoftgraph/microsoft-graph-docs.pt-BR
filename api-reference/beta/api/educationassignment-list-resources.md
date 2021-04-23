---
title: Listar educationAssignmentResources
description: Obter todos os recursos associados a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d770d17644462db110be021a541a0dfc28eacf9b
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961307"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="8c0ec-103">Listar educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="8c0ec-103">List educationAssignmentResources</span></span>

<span data-ttu-id="8c0ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c0ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c0ec-105">Obter todos os recursos associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-105">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c0ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c0ec-106">Permissions</span></span>
<span data-ttu-id="8c0ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c0ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c0ec-109">Permission type</span></span>      | <span data-ttu-id="8c0ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c0ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c0ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c0ec-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8c0ec-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c0ec-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8c0ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c0ec-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8c0ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-114">Not supported.</span></span>  |
|<span data-ttu-id="8c0ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c0ec-115">Application</span></span> | <span data-ttu-id="8c0ec-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c0ec-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8c0ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c0ec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c0ec-118">Optional query parameters</span></span>
<span data-ttu-id="8c0ec-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c0ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0ec-120">Request headers</span></span>
| <span data-ttu-id="8c0ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c0ec-121">Header</span></span>       | <span data-ttu-id="8c0ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c0ec-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c0ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c0ec-123">Authorization</span></span>  | <span data-ttu-id="8c0ec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c0ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0ec-126">Request body</span></span>
<span data-ttu-id="8c0ec-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8c0ec-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c0ec-128">Response</span></span>
<span data-ttu-id="8c0ec-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c0ec-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c0ec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c0ec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0ec-131">Request</span></span>
<span data-ttu-id="8c0ec-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c0ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
# <a name="c"></a>[<span data-ttu-id="8c0ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="8c0ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c0ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c0ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c0ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c0ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c0ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="8c0ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c0ec-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c0ec-138">Response</span></span>
<span data-ttu-id="8c0ec-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-139">The following is an example of the response.</span></span> 

><span data-ttu-id="8c0ec-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c0ec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
