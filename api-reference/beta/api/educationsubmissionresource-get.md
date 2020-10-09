---
title: Obter educationSubmissionResource
description: Recupera as propriedades de um recurso específico associado ao envio. Esse recurso está na lista de recursos de "trabalho" e deve ser considerado como trabalho em andamento por um aluno. Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição, caso tenha sido copiado da atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c0cac6fc194164cb13fb4e4bf473b00ed60def41
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403350"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="664dc-105">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="664dc-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="664dc-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="664dc-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="664dc-107">Recupera as propriedades de um recurso específico associado ao envio.</span><span class="sxs-lookup"><span data-stu-id="664dc-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="664dc-108">Esse recurso está na lista de recursos "trabalhando" e deve ser considerado como trabalho em andamento por um aluno.</span><span class="sxs-lookup"><span data-stu-id="664dc-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="664dc-109">Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição, caso tenha sido copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="664dc-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="664dc-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="664dc-110">Permissions</span></span>
<span data-ttu-id="664dc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="664dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="664dc-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="664dc-113">Permission type</span></span>      | <span data-ttu-id="664dc-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="664dc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="664dc-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="664dc-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="664dc-116">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="664dc-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="664dc-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="664dc-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="664dc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="664dc-118">Not supported.</span></span>  |
|<span data-ttu-id="664dc-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="664dc-119">Application</span></span> | <span data-ttu-id="664dc-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="664dc-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="664dc-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="664dc-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="664dc-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="664dc-122">Optional query parameters</span></span>
<span data-ttu-id="664dc-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="664dc-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="664dc-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="664dc-124">Request headers</span></span>
| <span data-ttu-id="664dc-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="664dc-125">Header</span></span>       | <span data-ttu-id="664dc-126">Valor</span><span class="sxs-lookup"><span data-stu-id="664dc-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="664dc-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="664dc-127">Authorization</span></span>  | <span data-ttu-id="664dc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="664dc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="664dc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="664dc-130">Request body</span></span>
<span data-ttu-id="664dc-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="664dc-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="664dc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="664dc-132">Response</span></span>
<span data-ttu-id="664dc-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="664dc-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="664dc-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="664dc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="664dc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="664dc-135">Request</span></span>
<span data-ttu-id="664dc-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="664dc-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="664dc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="664dc-137">Response</span></span>
<span data-ttu-id="664dc-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="664dc-138">The following is an example of the response.</span></span> 

><span data-ttu-id="664dc-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="664dc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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