---
title: Obter educationSubmittedSubmissionResource
description: Retorna um recurso enviado. Isso estará disponível para um professor após um estudante enviou e estarão disponível para o estudante após o professor lançou o envio.  Observe que professores podem deixar as anotações em alguns recursos.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e529231e6503b67390b7248228af84dc59b5f633
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513274"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="5cefd-105">Obter educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="5cefd-105">Get educationSubmittedSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cefd-106">Retorna um recurso enviado.</span><span class="sxs-lookup"><span data-stu-id="5cefd-106">Returns a submitted resource.</span></span> <span data-ttu-id="5cefd-107">Isso estará disponível para um professor após um estudante enviou e estarão disponível para o estudante após o professor lançou o envio.</span><span class="sxs-lookup"><span data-stu-id="5cefd-107">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="5cefd-108">Observe que professores podem deixar as anotações em alguns recursos.</span><span class="sxs-lookup"><span data-stu-id="5cefd-108">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cefd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5cefd-109">Permissions</span></span>
<span data-ttu-id="5cefd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cefd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cefd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cefd-112">Permission type</span></span>      | <span data-ttu-id="5cefd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5cefd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cefd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cefd-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="5cefd-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cefd-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5cefd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cefd-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5cefd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cefd-117">Not supported.</span></span>  |
|<span data-ttu-id="5cefd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cefd-118">Application</span></span> | <span data-ttu-id="5cefd-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cefd-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5cefd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cefd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5cefd-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5cefd-121">Optional query parameters</span></span>
<span data-ttu-id="5cefd-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5cefd-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cefd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cefd-123">Request headers</span></span>
| <span data-ttu-id="5cefd-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cefd-124">Header</span></span>       | <span data-ttu-id="5cefd-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5cefd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cefd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cefd-126">Authorization</span></span>  | <span data-ttu-id="5cefd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cefd-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cefd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cefd-129">Request body</span></span>
<span data-ttu-id="5cefd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cefd-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5cefd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cefd-131">Response</span></span>
<span data-ttu-id="5cefd-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cefd-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5cefd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cefd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cefd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cefd-134">Request</span></span>
<span data-ttu-id="5cefd-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cefd-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="5cefd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cefd-136">Response</span></span>
<span data-ttu-id="5cefd-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5cefd-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5cefd-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cefd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource"
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
      "@odata.type": "microsoft.graph.educationResource"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmittedsubmissionresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
