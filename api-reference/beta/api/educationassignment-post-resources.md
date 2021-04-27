---
title: Criar educationAssignmentResource
description: odata.type para indicar qual tipo de recurso está sendo criado. Observe que os recursos baseados em arquivo devem primeiro ser carregados para as atribuições **resourceFolder**.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8001af1c46ee374d47c9235f67080f87af74b4bc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044253"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="cdc78-104">Criar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="cdc78-104">Create educationAssignmentResource</span></span>

<span data-ttu-id="cdc78-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc78-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc78-106">Criar um [recurso de atribuição](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="cdc78-106">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="cdc78-107">O recurso em si tem um @odata.type para indicar qual tipo de recurso está sendo criado.</span><span class="sxs-lookup"><span data-stu-id="cdc78-107">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="cdc78-108">Observe que os recursos baseados em arquivo devem primeiro ser carregados para as atribuições **resourceFolder**.</span><span class="sxs-lookup"><span data-stu-id="cdc78-108">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc78-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdc78-109">Permissions</span></span>
<span data-ttu-id="cdc78-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc78-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdc78-112">Permission type</span></span>      | <span data-ttu-id="cdc78-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdc78-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdc78-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdc78-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="cdc78-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdc78-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="cdc78-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdc78-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cdc78-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc78-117">Not supported.</span></span>  |
|<span data-ttu-id="cdc78-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdc78-118">Application</span></span> | <span data-ttu-id="cdc78-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc78-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cdc78-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc78-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="cdc78-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc78-121">Request headers</span></span>
| <span data-ttu-id="cdc78-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdc78-122">Header</span></span>       | <span data-ttu-id="cdc78-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cdc78-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdc78-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdc78-124">Authorization</span></span>  | <span data-ttu-id="cdc78-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdc78-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdc78-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdc78-127">Content-Type</span></span>  | <span data-ttu-id="cdc78-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cdc78-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdc78-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc78-129">Request body</span></span>
<span data-ttu-id="cdc78-130">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="cdc78-130">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="cdc78-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc78-131">Response</span></span>
<span data-ttu-id="cdc78-132">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc78-132">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc78-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdc78-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdc78-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc78-134">Request</span></span>
<span data-ttu-id="cdc78-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdc78-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<span data-ttu-id="cdc78-136">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="cdc78-136">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cdc78-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc78-137">Response</span></span>
<span data-ttu-id="cdc78-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc78-138">The following is an example of the response.</span></span> 

><span data-ttu-id="cdc78-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cdc78-139">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "ignored",
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


