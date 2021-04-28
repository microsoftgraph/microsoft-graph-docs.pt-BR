---
title: Obter educationSubmittedSubmissionResource
description: Retorna um recurso enviado. Isso estará disponível para um professor ou um aplicativo com permissões de aplicativo depois que um aluno tiver enviado e estará disponível para o aluno depois que o professor tiver liberado o envio.  Observe que os professores podem deixar anotações em alguns recursos.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d2ce500e4a6a2dfc7cac779ddf3ab28e28476645
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061844"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="27371-105">Obter educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="27371-105">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="27371-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27371-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27371-107">Retorna um recurso enviado.</span><span class="sxs-lookup"><span data-stu-id="27371-107">Returns a submitted resource.</span></span> <span data-ttu-id="27371-108">Isso estará disponível para um professor ou um aplicativo com permissões de aplicativo depois que um aluno tiver enviado e estará disponível para o aluno depois que o professor tiver liberado o envio.</span><span class="sxs-lookup"><span data-stu-id="27371-108">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="27371-109">Observe que os professores podem deixar anotações em alguns recursos.</span><span class="sxs-lookup"><span data-stu-id="27371-109">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="27371-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="27371-110">Permissions</span></span>
<span data-ttu-id="27371-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27371-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27371-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27371-113">Permission type</span></span>      | <span data-ttu-id="27371-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27371-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27371-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27371-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="27371-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27371-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="27371-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27371-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="27371-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27371-118">Not supported.</span></span>  |
|<span data-ttu-id="27371-119">Application\*</span><span class="sxs-lookup"><span data-stu-id="27371-119">Application\*</span></span> | <span data-ttu-id="27371-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27371-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="27371-121">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="27371-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="27371-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27371-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27371-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27371-123">Optional query parameters</span></span>
<span data-ttu-id="27371-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27371-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27371-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27371-125">Request headers</span></span>
| <span data-ttu-id="27371-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27371-126">Header</span></span>       | <span data-ttu-id="27371-127">Valor</span><span class="sxs-lookup"><span data-stu-id="27371-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27371-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="27371-128">Authorization</span></span>  | <span data-ttu-id="27371-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27371-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27371-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27371-131">Request body</span></span>
<span data-ttu-id="27371-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27371-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="27371-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27371-133">Response</span></span>
<span data-ttu-id="27371-134">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27371-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27371-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27371-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27371-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27371-136">Request</span></span>
<span data-ttu-id="27371-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27371-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="27371-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="27371-138">Response</span></span>
<span data-ttu-id="27371-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27371-139">The following is an example of the response.</span></span> 

><span data-ttu-id="27371-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27371-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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