---
title: Obter educationSubmittedSubmissionResource
description: Retorna um recurso enviado. Isso estará disponível para um professor após um estudante enviou e estarão disponível para o estudante após o professor lançou o envio.  Observe que professores podem deixar as anotações em alguns recursos.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc7b6f9f0a224cf7a9c1e1c069756d8c83e08ba8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926229"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="ec4bf-105">Obter educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="ec4bf-105">Get educationSubmittedSubmissionResource</span></span>

> <span data-ttu-id="ec4bf-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec4bf-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec4bf-108">Retorna um recurso enviado.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-108">Returns a submitted resource.</span></span> <span data-ttu-id="ec4bf-109">Isso estará disponível para um professor após um estudante enviou e estarão disponível para o estudante após o professor lançou o envio.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-109">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="ec4bf-110">Observe que professores podem deixar as anotações em alguns recursos.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-110">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec4bf-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="ec4bf-111">Permissions</span></span>
<span data-ttu-id="ec4bf-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec4bf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec4bf-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec4bf-114">Permission type</span></span>      | <span data-ttu-id="ec4bf-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec4bf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec4bf-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec4bf-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec4bf-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec4bf-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ec4bf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec4bf-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ec4bf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-119">Not supported.</span></span>  |
|<span data-ttu-id="ec4bf-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec4bf-120">Application</span></span> | <span data-ttu-id="ec4bf-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ec4bf-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec4bf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec4bf-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec4bf-123">Optional query parameters</span></span>
<span data-ttu-id="ec4bf-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec4bf-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec4bf-125">Request headers</span></span>
| <span data-ttu-id="ec4bf-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec4bf-126">Header</span></span>       | <span data-ttu-id="ec4bf-127">Valor</span><span class="sxs-lookup"><span data-stu-id="ec4bf-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec4bf-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec4bf-128">Authorization</span></span>  | <span data-ttu-id="ec4bf-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec4bf-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec4bf-131">Request body</span></span>
<span data-ttu-id="ec4bf-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ec4bf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec4bf-133">Response</span></span>
<span data-ttu-id="ec4bf-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec4bf-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec4bf-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec4bf-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec4bf-136">Request</span></span>
<span data-ttu-id="ec4bf-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="ec4bf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec4bf-138">Response</span></span>
<span data-ttu-id="ec4bf-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-139">The following is an example of the response.</span></span> 

><span data-ttu-id="ec4bf-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec4bf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
