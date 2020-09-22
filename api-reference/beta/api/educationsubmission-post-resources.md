---
title: Criar educationSubmissionResource
description: 'Adiciona um recurso à lista de recursos. Esta ação só pode ser feita pelo aluno a quem esse envio é atribuído. Esta ação não será bem-sucedida se o sinalizador **allowStudentsToAddResources** não estiver definido como true. Se o chamador quiser criar um novo recurso baseado em arquivo, o arquivo deverá ser carregado na pasta recursos que está associada ao envio. Se o arquivo não existir ou não estiver nessa pasta, a solicitação POST falhará. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d078cfb0f5e81cd245058b3952a74cfe5dd34836
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007230"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="ff74b-107">Criar educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="ff74b-107">Create educationSubmissionResource</span></span>

<span data-ttu-id="ff74b-108">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ff74b-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff74b-109">Adiciona um recurso à lista de recursos.</span><span class="sxs-lookup"><span data-stu-id="ff74b-109">Adds a resource to the resources list.</span></span> <span data-ttu-id="ff74b-110">Esta ação só pode ser feita pelo aluno a quem esse envio é atribuído.</span><span class="sxs-lookup"><span data-stu-id="ff74b-110">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="ff74b-111">Esta ação não será bem-sucedida se o sinalizador **allowStudentsToAddResources** não estiver definido como true.</span><span class="sxs-lookup"><span data-stu-id="ff74b-111">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="ff74b-112">Se o chamador quiser criar um novo recurso baseado em arquivo, o arquivo deverá ser carregado na pasta recursos que está associada ao envio.</span><span class="sxs-lookup"><span data-stu-id="ff74b-112">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="ff74b-113">Se o arquivo não existir ou não estiver nessa pasta, a solicitação POST falhará.</span><span class="sxs-lookup"><span data-stu-id="ff74b-113">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ff74b-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff74b-114">Permissions</span></span>
<span data-ttu-id="ff74b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff74b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff74b-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff74b-117">Permission type</span></span>      | <span data-ttu-id="ff74b-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff74b-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff74b-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff74b-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff74b-120">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff74b-120">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ff74b-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff74b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff74b-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff74b-122">Not supported.</span></span>  |
|<span data-ttu-id="ff74b-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff74b-123">Application</span></span> | <span data-ttu-id="ff74b-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff74b-124">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ff74b-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff74b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="ff74b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff74b-126">Request headers</span></span>
| <span data-ttu-id="ff74b-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff74b-127">Header</span></span>       | <span data-ttu-id="ff74b-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ff74b-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff74b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff74b-129">Authorization</span></span>  | <span data-ttu-id="ff74b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff74b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff74b-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff74b-132">Content-Type</span></span>  | <span data-ttu-id="ff74b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ff74b-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff74b-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff74b-134">Request body</span></span>
<span data-ttu-id="ff74b-135">No corpo da solicitação, forneça uma representação JSON do objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) .</span><span class="sxs-lookup"><span data-stu-id="ff74b-135">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ff74b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff74b-136">Response</span></span>
<span data-ttu-id="ff74b-137">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff74b-137">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff74b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff74b-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff74b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff74b-139">Request</span></span>
<span data-ttu-id="ff74b-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff74b-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources
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

##### <a name="response"></a><span data-ttu-id="ff74b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff74b-141">Response</span></span>
<span data-ttu-id="ff74b-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff74b-142">The following is an example of the response.</span></span> 

><span data-ttu-id="ff74b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff74b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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


