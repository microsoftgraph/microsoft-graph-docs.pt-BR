---
title: Criar educationAssignmentResource
description: Criar um recurso de atribuição de educação.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 20719f61e7b01c42bd6615ef2c0bb032fe8b5c36
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912156"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="e5326-103">Criar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e5326-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="e5326-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5326-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5326-105">Criar um [recurso de atribuição](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="e5326-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> 

<span data-ttu-id="e5326-106">Cada recurso tem uma propriedade @odata.type para indicar qual tipo de recurso está sendo criado.</span><span class="sxs-lookup"><span data-stu-id="e5326-106">Every resource has an @odata.type property to indicate which type of resource is being created.</span></span> 

[!IMPORTANT] 
<span data-ttu-id="e5326-107">Upload recurso baseado em arquivo para as atribuições `resourcesFolder` antes de criar o recurso.</span><span class="sxs-lookup"><span data-stu-id="e5326-107">Upload file-based resource to the assignments `resourcesFolder` before creating the resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e5326-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5326-108">Permissions</span></span>
<span data-ttu-id="e5326-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5326-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5326-111">Permission type</span></span>      | <span data-ttu-id="e5326-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5326-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5326-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5326-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5326-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5326-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e5326-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5326-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e5326-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5326-116">Not supported.</span></span>  |
|<span data-ttu-id="e5326-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5326-117">Application</span></span> | <span data-ttu-id="e5326-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5326-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e5326-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5326-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="e5326-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5326-120">Request headers</span></span>
| <span data-ttu-id="e5326-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5326-121">Header</span></span>       | <span data-ttu-id="e5326-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5326-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5326-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5326-123">Authorization</span></span>  | <span data-ttu-id="e5326-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5326-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5326-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5326-126">Content-Type</span></span>  | <span data-ttu-id="e5326-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5326-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5326-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5326-128">Request body</span></span>
<span data-ttu-id="e5326-129">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="e5326-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e5326-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5326-130">Response</span></span>
<span data-ttu-id="e5326-131">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5326-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5326-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5326-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5326-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5326-133">Request</span></span>
<span data-ttu-id="e5326-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5326-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="e5326-135">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="e5326-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="e5326-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5326-136">Response</span></span>
<span data-ttu-id="e5326-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5326-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e5326-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5326-138">**Note:** The response object shown here might be shortened for readability.</span></span>


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


