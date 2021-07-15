---
title: Criar educationAssignmentResource
description: Criar um recurso de atribuição de educação.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: af94dc0e6e9a2c2cef30a177509bf32f50faa3ae
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439865"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="bcc1e-103">Criar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="bcc1e-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="bcc1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcc1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcc1e-105">Criar um [recurso de atribuição](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="bcc1e-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="bcc1e-106">O recurso em si tem um @odata.type para indicar qual tipo de recurso está sendo criado.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="bcc1e-107">Observe que os recursos baseados em arquivo devem primeiro ser carregados para as atribuições **resourceFolder**.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcc1e-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bcc1e-108">Permissions</span></span>
<span data-ttu-id="bcc1e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc1e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcc1e-111">Permission type</span></span>      | <span data-ttu-id="bcc1e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcc1e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcc1e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcc1e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="bcc1e-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc1e-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bcc1e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcc1e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bcc1e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-116">Not supported.</span></span>  |
|<span data-ttu-id="bcc1e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcc1e-117">Application</span></span> | <span data-ttu-id="bcc1e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="bcc1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc1e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="bcc1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc1e-120">Request headers</span></span>
| <span data-ttu-id="bcc1e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcc1e-121">Header</span></span>       | <span data-ttu-id="bcc1e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bcc1e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcc1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcc1e-123">Authorization</span></span>  | <span data-ttu-id="bcc1e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bcc1e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcc1e-126">Content-Type</span></span>  | <span data-ttu-id="bcc1e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc1e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcc1e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc1e-128">Request body</span></span>
<span data-ttu-id="bcc1e-129">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="bcc1e-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="bcc1e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcc1e-130">Response</span></span>
<span data-ttu-id="bcc1e-131">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc1e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcc1e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcc1e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc1e-133">Request</span></span>
<span data-ttu-id="bcc1e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="bcc1e-135">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="bcc1e-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="bcc1e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcc1e-136">Response</span></span>
<span data-ttu-id="bcc1e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="bcc1e-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bcc1e-138">**Note:** The response object shown here might be shortened for readability.</span></span>


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


