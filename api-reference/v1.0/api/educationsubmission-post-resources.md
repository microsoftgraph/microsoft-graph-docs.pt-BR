---
title: Criar educationSubmissionResource
description: Adicione um recurso à lista de recursos de envio.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a5b883c4b25b24f51defcc7d13a8f8e657e2ad48
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912140"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="a94f8-103">Criar educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="a94f8-103">Create educationSubmissionResource</span></span>

<span data-ttu-id="a94f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a94f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a94f8-105">Adicione um recurso à lista de recursos de envio.</span><span class="sxs-lookup"><span data-stu-id="a94f8-105">Add a resource to the submission resource list.</span></span> 

<span data-ttu-id="a94f8-106">Essa ação só pode ser feita pelo aluno ao qual esse envio é atribuído.</span><span class="sxs-lookup"><span data-stu-id="a94f8-106">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="a94f8-107">Essa ação não terá êxito **se o sinalizador allowStudentsToAddResources** não estiver definido como `true` .</span><span class="sxs-lookup"><span data-stu-id="a94f8-107">This action will not succeed if the **allowStudentsToAddResources** flag isn't set to `true`.</span></span> <span data-ttu-id="a94f8-108">Se o chamador quiser criar um novo recurso baseado em arquivo, o arquivo deverá ser carregado na pasta de recursos associada ao envio.</span><span class="sxs-lookup"><span data-stu-id="a94f8-108">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="a94f8-109">Se o arquivo não existir ou não estiver nessa pasta, a solicitação POST falhará.</span><span class="sxs-lookup"><span data-stu-id="a94f8-109">If the file does not exist or isn't in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a94f8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a94f8-110">Permissions</span></span>
<span data-ttu-id="a94f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a94f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a94f8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a94f8-113">Permission type</span></span>      | <span data-ttu-id="a94f8-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a94f8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a94f8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a94f8-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="a94f8-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a94f8-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a94f8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a94f8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a94f8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a94f8-118">Not supported.</span></span>  |
|<span data-ttu-id="a94f8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a94f8-119">Application</span></span> | <span data-ttu-id="a94f8-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a94f8-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a94f8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a94f8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="request-headers"></a><span data-ttu-id="a94f8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a94f8-122">Request headers</span></span>
| <span data-ttu-id="a94f8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a94f8-123">Header</span></span>       | <span data-ttu-id="a94f8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a94f8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a94f8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a94f8-125">Authorization</span></span>  | <span data-ttu-id="a94f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a94f8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a94f8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a94f8-128">Content-Type</span></span>  | <span data-ttu-id="a94f8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a94f8-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a94f8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a94f8-130">Request body</span></span>
<span data-ttu-id="a94f8-131">No corpo da solicitação, fornece uma representação JSON do [objeto educationSubmissionResource.](../resources/educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="a94f8-131">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a94f8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a94f8-132">Response</span></span>
<span data-ttu-id="a94f8-133">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a94f8-133">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a94f8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a94f8-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a94f8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a94f8-135">Request</span></span>
<span data-ttu-id="a94f8-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a94f8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
  },
  "@odata.type": "microsoft.graph.educationResource"
}
```

### <a name="response"></a><span data-ttu-id="a94f8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a94f8-137">Response</span></span>
<span data-ttu-id="a94f8-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a94f8-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a94f8-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a94f8-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


