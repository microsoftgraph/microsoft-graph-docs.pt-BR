---
title: Obter educationSubmissionResource
description: Recupera as propriedades de um recurso específico associado ao envio. Esse recurso está na lista de recursos "trabalhando" e deve ser considerado trabalho em processo por um aluno. Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição se tiver sido copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6f12b9b1739f844b5ef41e99942c3063f0cec95
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470351"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="d567a-105">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d567a-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="d567a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d567a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d567a-107">Recupera as propriedades de um recurso específico associado ao envio.</span><span class="sxs-lookup"><span data-stu-id="d567a-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="d567a-108">Esse recurso está na lista de recursos "trabalhando" e deve ser considerado trabalho em processo por um aluno.</span><span class="sxs-lookup"><span data-stu-id="d567a-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="d567a-109">Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição se tiver sido copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d567a-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d567a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d567a-110">Permissions</span></span>
<span data-ttu-id="d567a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d567a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d567a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d567a-113">Permission type</span></span>      | <span data-ttu-id="d567a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d567a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d567a-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d567a-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d567a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d567a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d567a-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d567a-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d567a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d567a-118">Not supported.</span></span>  |
|<span data-ttu-id="d567a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d567a-119">Application</span></span> | <span data-ttu-id="d567a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d567a-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d567a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d567a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d567a-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d567a-122">Optional query parameters</span></span>
<span data-ttu-id="d567a-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d567a-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d567a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d567a-124">Request headers</span></span>
| <span data-ttu-id="d567a-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d567a-125">Header</span></span>       | <span data-ttu-id="d567a-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d567a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d567a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d567a-127">Authorization</span></span>  | <span data-ttu-id="d567a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d567a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d567a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d567a-130">Request body</span></span>
<span data-ttu-id="d567a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d567a-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d567a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d567a-132">Response</span></span>
<span data-ttu-id="d567a-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d567a-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d567a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d567a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d567a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d567a-135">Request</span></span>
<span data-ttu-id="d567a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d567a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d567a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d567a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="d567a-138">C#</span><span class="sxs-lookup"><span data-stu-id="d567a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d567a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d567a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d567a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d567a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d567a-141">Java</span><span class="sxs-lookup"><span data-stu-id="d567a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d567a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d567a-142">Response</span></span>
<span data-ttu-id="d567a-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d567a-143">The following is an example of the response.</span></span> 

><span data-ttu-id="d567a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d567a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
