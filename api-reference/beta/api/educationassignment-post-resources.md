---
title: Criar educationAssignmentResource
description: OData.Type para indicar qual tipo de recurso está sendo criado. Observe que recursos baseados no arquivo devem ser carregados primeiro para as atribuições **resourceFolder**.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 34e8740336acbef056ec0b3703547de51fdc42ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527987"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="55e25-104">Criar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="55e25-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e25-105">Crie um [recurso de atribuição](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="55e25-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="55e25-106">O recurso propriamente dito tem um @odata.type para indicar qual tipo de recurso está sendo criado.</span><span class="sxs-lookup"><span data-stu-id="55e25-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="55e25-107">Observe que recursos baseados no arquivo devem ser carregados primeiro para as atribuições **resourceFolder**.</span><span class="sxs-lookup"><span data-stu-id="55e25-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="55e25-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="55e25-108">Permissions</span></span>
<span data-ttu-id="55e25-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55e25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55e25-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55e25-111">Permission type</span></span>      | <span data-ttu-id="55e25-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55e25-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55e25-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55e25-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="55e25-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55e25-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="55e25-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55e25-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="55e25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55e25-116">Not supported.</span></span>  |
|<span data-ttu-id="55e25-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55e25-117">Application</span></span> | <span data-ttu-id="55e25-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55e25-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="55e25-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55e25-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="55e25-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55e25-120">Request headers</span></span>
| <span data-ttu-id="55e25-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55e25-121">Header</span></span>       | <span data-ttu-id="55e25-122">Valor</span><span class="sxs-lookup"><span data-stu-id="55e25-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55e25-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55e25-123">Authorization</span></span>  | <span data-ttu-id="55e25-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55e25-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="55e25-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55e25-126">Content-Type</span></span>  | <span data-ttu-id="55e25-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55e25-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55e25-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55e25-128">Request body</span></span>
<span data-ttu-id="55e25-129">No corpo da solicitação, fornece uma representação JSON do objeto [educationAssignmentResource](../resources/educationassignmentresource.md) .</span><span class="sxs-lookup"><span data-stu-id="55e25-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="55e25-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="55e25-130">Response</span></span>
<span data-ttu-id="55e25-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55e25-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55e25-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55e25-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55e25-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55e25-133">Request</span></span>
<span data-ttu-id="55e25-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55e25-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="55e25-135">No corpo da solicitação, fornece uma representação JSON do objeto [educationAssignmentResource](../resources/educationassignmentresource.md) .</span><span class="sxs-lookup"><span data-stu-id="55e25-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="55e25-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="55e25-136">Response</span></span>
<span data-ttu-id="55e25-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55e25-137">The following is an example of the response.</span></span> 

><span data-ttu-id="55e25-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55e25-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55e25-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55e25-139">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
