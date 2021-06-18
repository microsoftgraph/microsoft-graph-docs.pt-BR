---
title: Criar educationAssignmentResource
description: Criar um recurso de atribuição de educação.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2febd840a6ba93f28f38d66d94a2e8f69a526ca2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992776"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="8b062-103">Criar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="8b062-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="8b062-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b062-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b062-105">Criar um [recurso de atribuição](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="8b062-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> 

<span data-ttu-id="8b062-106">Cada recurso tem uma propriedade @odata.type para indicar qual tipo de recurso está sendo criado.</span><span class="sxs-lookup"><span data-stu-id="8b062-106">Every resource has an @odata.type property to indicate which type of resource is being created.</span></span> 

[!IMPORTANT] 
<span data-ttu-id="8b062-107">Upload recurso baseado em arquivo para as atribuições `resourcesFolder` antes de criar o recurso.</span><span class="sxs-lookup"><span data-stu-id="8b062-107">Upload file-based resource to the assignments `resourcesFolder` before creating the resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8b062-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b062-108">Permissions</span></span>
<span data-ttu-id="8b062-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b062-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b062-111">Permission type</span></span>      | <span data-ttu-id="8b062-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b062-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b062-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b062-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8b062-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b062-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8b062-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b062-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8b062-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b062-116">Not supported.</span></span>  |
|<span data-ttu-id="8b062-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b062-117">Application</span></span> | <span data-ttu-id="8b062-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b062-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8b062-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b062-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="8b062-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b062-120">Request headers</span></span>
| <span data-ttu-id="8b062-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b062-121">Header</span></span>       | <span data-ttu-id="8b062-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8b062-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b062-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b062-123">Authorization</span></span>  | <span data-ttu-id="8b062-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b062-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b062-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b062-126">Content-Type</span></span>  | <span data-ttu-id="8b062-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8b062-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b062-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b062-128">Request body</span></span>
<span data-ttu-id="8b062-129">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="8b062-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="8b062-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b062-130">Response</span></span>
<span data-ttu-id="8b062-131">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b062-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b062-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b062-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b062-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b062-133">Request</span></span>
<span data-ttu-id="8b062-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b062-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b062-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b062-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "educationLinkResource"
  }
}

```
# <a name="c"></a>[<span data-ttu-id="8b062-136">C#</span><span class="sxs-lookup"><span data-stu-id="8b062-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationassignmentresource-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b062-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b062-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationassignmentresource-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b062-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b062-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationassignmentresource-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b062-139">Java</span><span class="sxs-lookup"><span data-stu-id="8b062-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationassignmentresource-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8b062-140">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="8b062-140">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="8b062-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b062-141">Response</span></span>
<span data-ttu-id="8b062-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b062-142">The following is an example of the response.</span></span> 

><span data-ttu-id="8b062-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b062-143">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


