---
title: Obter educationSubmittedSubmissionResource
description: Recupere um recurso enviado.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00c9bb49c43dd809945166a6dca4a05a76a87b5f
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912215"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="7d72c-103">Obter educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="7d72c-103">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="7d72c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d72c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d72c-105">Recuperar um [recurso enviado](../resources/educationsubmissionresource.md).</span><span class="sxs-lookup"><span data-stu-id="7d72c-105">Retrieve a [submitted resource](../resources/educationsubmissionresource.md).</span></span> 

<span data-ttu-id="7d72c-106">Isso estará disponível para um professor ou um aplicativo com permissões de aplicativo depois que um aluno tiver enviado e estará disponível para o aluno depois que o professor tiver liberado o envio.</span><span class="sxs-lookup"><span data-stu-id="7d72c-106">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="7d72c-107">Observe que os professores podem deixar anotações em alguns recursos.</span><span class="sxs-lookup"><span data-stu-id="7d72c-107">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d72c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d72c-108">Permissions</span></span>
<span data-ttu-id="7d72c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d72c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d72c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d72c-111">Permission type</span></span>      | <span data-ttu-id="7d72c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d72c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d72c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d72c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="7d72c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d72c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7d72c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d72c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7d72c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d72c-116">Not supported.</span></span>  |
|<span data-ttu-id="7d72c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d72c-117">Application</span></span> | <span data-ttu-id="7d72c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d72c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7d72c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d72c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d72c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d72c-120">Optional query parameters</span></span>
<span data-ttu-id="7d72c-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d72c-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d72c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d72c-122">Request headers</span></span>
| <span data-ttu-id="7d72c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d72c-123">Header</span></span>       | <span data-ttu-id="7d72c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7d72c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d72c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d72c-125">Authorization</span></span>  | <span data-ttu-id="7d72c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d72c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d72c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d72c-128">Request body</span></span>
<span data-ttu-id="7d72c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d72c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d72c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d72c-130">Response</span></span>
<span data-ttu-id="7d72c-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d72c-131">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span> <span data-ttu-id="7d72c-132">Caso contrário, retorna `404 Not found` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d72c-132">Otherwise, returns a `404 Not found` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d72c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d72c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d72c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d72c-134">Request</span></span>
<span data-ttu-id="7d72c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d72c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/f973bc68-2adb-4cf7-8b15-a57a1936b60c/assignments/8b890b42-a1df-478b-bff5-6814afb1afc2/submissions/6d71b348-898a-40cd-8e71-35127eed97f5/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
### <a name="response"></a><span data-ttu-id="7d72c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d72c-136">Response</span></span>
<span data-ttu-id="7d72c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d72c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="7d72c-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d72c-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource"
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
