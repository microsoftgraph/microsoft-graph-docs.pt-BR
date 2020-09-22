---
title: Obter educationSubmissionResource
description: Recupera as propriedades de um recurso específico associado ao envio. Esse recurso está na lista de recursos de "trabalho" e deve ser considerado como trabalho em andamento por um aluno. Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição, caso tenha sido copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5968f189dd3eea8a976cdcb6c141742b19ef4618
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991300"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="d22fb-105">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d22fb-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="d22fb-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d22fb-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d22fb-107">Recupera as propriedades de um recurso específico associado ao envio.</span><span class="sxs-lookup"><span data-stu-id="d22fb-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="d22fb-108">Esse recurso está na lista de recursos "trabalhando" e deve ser considerado como trabalho em andamento por um aluno.</span><span class="sxs-lookup"><span data-stu-id="d22fb-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="d22fb-109">Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição, caso tenha sido copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d22fb-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d22fb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d22fb-110">Permissions</span></span>
<span data-ttu-id="d22fb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d22fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d22fb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d22fb-113">Permission type</span></span>      | <span data-ttu-id="d22fb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d22fb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d22fb-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d22fb-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d22fb-116">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d22fb-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d22fb-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d22fb-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d22fb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d22fb-118">Not supported.</span></span>  |
|<span data-ttu-id="d22fb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d22fb-119">Application</span></span> | <span data-ttu-id="d22fb-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d22fb-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d22fb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d22fb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d22fb-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d22fb-122">Optional query parameters</span></span>
<span data-ttu-id="d22fb-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d22fb-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d22fb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d22fb-124">Request headers</span></span>
| <span data-ttu-id="d22fb-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d22fb-125">Header</span></span>       | <span data-ttu-id="d22fb-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d22fb-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d22fb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d22fb-127">Authorization</span></span>  | <span data-ttu-id="d22fb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d22fb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d22fb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d22fb-130">Request body</span></span>
<span data-ttu-id="d22fb-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d22fb-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d22fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d22fb-132">Response</span></span>
<span data-ttu-id="d22fb-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d22fb-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d22fb-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d22fb-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d22fb-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d22fb-135">Request</span></span>
<span data-ttu-id="d22fb-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d22fb-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="d22fb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d22fb-137">Response</span></span>
<span data-ttu-id="d22fb-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d22fb-138">The following is an example of the response.</span></span> 

><span data-ttu-id="d22fb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d22fb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->


