---
title: Obter educationSubmissionResource
description: Recupere as propriedades de um recurso específico associado ao envio.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 086f6c965252b528377feaabbd06ad2110c67139
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912126"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="c6c94-103">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="c6c94-103">Get educationSubmissionResource</span></span>

<span data-ttu-id="c6c94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6c94-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6c94-105">Recupere as propriedades de um recurso específico associado a um [envio](../resources/educationsubmissionresource.md).</span><span class="sxs-lookup"><span data-stu-id="c6c94-105">Retrieve the properties of a specific resource associated with a [submission](../resources/educationsubmissionresource.md).</span></span> 

<span data-ttu-id="c6c94-106">Esse recurso está na lista de recursos "trabalhando" e deve ser considerado trabalho em processo por um aluno.</span><span class="sxs-lookup"><span data-stu-id="c6c94-106">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="c6c94-107">Esse recurso é empacotado com um possível ponteiro de volta para o recurso de atribuição se tiver sido copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c6c94-107">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6c94-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6c94-108">Permissions</span></span>
<span data-ttu-id="c6c94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6c94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6c94-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6c94-111">Permission type</span></span>      | <span data-ttu-id="c6c94-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6c94-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6c94-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6c94-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c6c94-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c94-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c6c94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6c94-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6c94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c94-116">Not supported.</span></span>  |
|<span data-ttu-id="c6c94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6c94-117">Application</span></span> | <span data-ttu-id="c6c94-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c94-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c6c94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6c94-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6c94-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6c94-120">Optional query parameters</span></span>
<span data-ttu-id="c6c94-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c94-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6c94-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c94-122">Request headers</span></span>
| <span data-ttu-id="c6c94-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6c94-123">Header</span></span>       | <span data-ttu-id="c6c94-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c6c94-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6c94-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6c94-125">Authorization</span></span>  | <span data-ttu-id="c6c94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6c94-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6c94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c94-128">Request body</span></span>
<span data-ttu-id="c6c94-129">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="c6c94-129">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c6c94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c94-130">Response</span></span>
<span data-ttu-id="c6c94-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c94-131">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6c94-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6c94-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6c94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c94-133">Request</span></span>
<span data-ttu-id="c6c94-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6c94-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```

### <a name="response"></a><span data-ttu-id="c6c94-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c94-135">Response</span></span>
<span data-ttu-id="c6c94-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c94-136">The following is an example of the response.</span></span> 

><span data-ttu-id="c6c94-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c6c94-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
