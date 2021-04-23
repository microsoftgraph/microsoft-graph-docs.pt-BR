---
title: Obter educationSubmittedSubmissionResource
description: Retorna um recurso enviado. Isso estará disponível para um professor ou um aplicativo com permissões de aplicativo depois que um aluno tiver enviado e estará disponível para o aluno depois que o professor tiver liberado o envio.  Observe que os professores podem deixar anotações em alguns recursos.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3a7db3962a2dbc7e012c1e89080008efcd228e52
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961111"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="79149-105">Obter educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="79149-105">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="79149-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79149-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79149-107">Retorna um recurso enviado.</span><span class="sxs-lookup"><span data-stu-id="79149-107">Returns a submitted resource.</span></span> <span data-ttu-id="79149-108">Isso estará disponível para um professor ou um aplicativo com permissões de aplicativo depois que um aluno tiver enviado e estará disponível para o aluno depois que o professor tiver liberado o envio.</span><span class="sxs-lookup"><span data-stu-id="79149-108">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="79149-109">Observe que os professores podem deixar anotações em alguns recursos.</span><span class="sxs-lookup"><span data-stu-id="79149-109">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="79149-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="79149-110">Permissions</span></span>
<span data-ttu-id="79149-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79149-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79149-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79149-113">Permission type</span></span>      | <span data-ttu-id="79149-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79149-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79149-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79149-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="79149-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79149-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="79149-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79149-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="79149-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79149-118">Not supported.</span></span>  |
|<span data-ttu-id="79149-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79149-119">Application</span></span> | <span data-ttu-id="79149-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79149-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="79149-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79149-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79149-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79149-122">Optional query parameters</span></span>
<span data-ttu-id="79149-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79149-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79149-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79149-124">Request headers</span></span>
| <span data-ttu-id="79149-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79149-125">Header</span></span>       | <span data-ttu-id="79149-126">Valor</span><span class="sxs-lookup"><span data-stu-id="79149-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79149-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="79149-127">Authorization</span></span>  | <span data-ttu-id="79149-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79149-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79149-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79149-130">Request body</span></span>
<span data-ttu-id="79149-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79149-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="79149-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="79149-132">Response</span></span>
<span data-ttu-id="79149-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79149-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79149-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79149-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79149-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79149-135">Request</span></span>
<span data-ttu-id="79149-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79149-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="79149-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="79149-137">Response</span></span>
<span data-ttu-id="79149-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79149-138">The following is an example of the response.</span></span> 

><span data-ttu-id="79149-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79149-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->