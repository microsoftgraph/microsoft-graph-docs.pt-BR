---
title: Obter educationSubmissionResource
description: Recupera as propriedades de um recurso específico associado ao envio. Esse recurso está na lista de recursos de "trabalho" e deve ser considerado como trabalho em andamento por um aluno. Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição, caso tenha sido copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b76d697afa842fe5315792d803e9b704a628a0b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464681"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="8a2de-105">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="8a2de-105">Get educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a2de-106">Recupera as propriedades de um recurso específico associado ao envio.</span><span class="sxs-lookup"><span data-stu-id="8a2de-106">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="8a2de-107">Esse recurso está na lista de recursos "trabalhando" e deve ser considerado como trabalho em andamento por um aluno.</span><span class="sxs-lookup"><span data-stu-id="8a2de-107">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="8a2de-108">Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição, caso tenha sido copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="8a2de-108">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a2de-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a2de-109">Permissions</span></span>
<span data-ttu-id="8a2de-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a2de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a2de-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a2de-112">Permission type</span></span>      | <span data-ttu-id="8a2de-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a2de-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a2de-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a2de-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a2de-115">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a2de-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8a2de-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a2de-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a2de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a2de-117">Not supported.</span></span>  |
|<span data-ttu-id="8a2de-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a2de-118">Application</span></span> | <span data-ttu-id="8a2de-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a2de-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a2de-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a2de-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a2de-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8a2de-121">Optional query parameters</span></span>
<span data-ttu-id="8a2de-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8a2de-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a2de-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a2de-123">Request headers</span></span>
| <span data-ttu-id="8a2de-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a2de-124">Header</span></span>       | <span data-ttu-id="8a2de-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8a2de-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a2de-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a2de-126">Authorization</span></span>  | <span data-ttu-id="8a2de-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a2de-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a2de-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a2de-129">Request body</span></span>
<span data-ttu-id="8a2de-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a2de-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8a2de-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a2de-131">Response</span></span>
<span data-ttu-id="8a2de-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a2de-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a2de-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a2de-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a2de-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a2de-134">Request</span></span>
<span data-ttu-id="8a2de-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a2de-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="8a2de-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a2de-136">Response</span></span>
<span data-ttu-id="8a2de-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a2de-137">The following is an example of the response.</span></span> 

><span data-ttu-id="8a2de-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a2de-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
