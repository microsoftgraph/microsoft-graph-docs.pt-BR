---
title: Criar educationAssignmentResource
description: OData.Type para indicar qual tipo de recurso está sendo criado. Observe que recursos baseados no arquivo devem ser carregados primeiro para as atribuições **resourceFolder**.
ms.openlocfilehash: a2bb810d16c2d0a46fc2e2f4a5938b5779df24af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034990"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="ec48a-104">Criar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="ec48a-104">Create educationAssignmentResource</span></span>

> <span data-ttu-id="ec48a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec48a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec48a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec48a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec48a-107">Crie um [recurso de atribuição](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="ec48a-107">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="ec48a-108">O recurso propriamente dito tem um @odata.type para indicar qual tipo de recurso está sendo criado.</span><span class="sxs-lookup"><span data-stu-id="ec48a-108">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="ec48a-109">Observe que recursos baseados no arquivo devem ser carregados primeiro para as atribuições **resourceFolder**.</span><span class="sxs-lookup"><span data-stu-id="ec48a-109">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec48a-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="ec48a-110">Permissions</span></span>
<span data-ttu-id="ec48a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec48a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec48a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec48a-113">Permission type</span></span>      | <span data-ttu-id="ec48a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec48a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec48a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec48a-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec48a-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec48a-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ec48a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec48a-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ec48a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec48a-118">Not supported.</span></span>  |
|<span data-ttu-id="ec48a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec48a-119">Application</span></span> | <span data-ttu-id="ec48a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec48a-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ec48a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec48a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="ec48a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec48a-122">Request headers</span></span>
| <span data-ttu-id="ec48a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec48a-123">Header</span></span>       | <span data-ttu-id="ec48a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ec48a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec48a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec48a-125">Authorization</span></span>  | <span data-ttu-id="ec48a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec48a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec48a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec48a-128">Content-Type</span></span>  | <span data-ttu-id="ec48a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ec48a-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec48a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec48a-130">Request body</span></span>
<span data-ttu-id="ec48a-131">No corpo da solicitação, fornece uma representação JSON do objeto [educationAssignmentResource](../resources/educationassignmentresource.md) .</span><span class="sxs-lookup"><span data-stu-id="ec48a-131">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ec48a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec48a-132">Response</span></span>
<span data-ttu-id="ec48a-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec48a-133">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec48a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec48a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec48a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec48a-135">Request</span></span>
<span data-ttu-id="ec48a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec48a-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="ec48a-137">No corpo da solicitação, fornece uma representação JSON do objeto [educationAssignmentResource](../resources/educationassignmentresource.md) .</span><span class="sxs-lookup"><span data-stu-id="ec48a-137">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ec48a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec48a-138">Response</span></span>
<span data-ttu-id="ec48a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec48a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="ec48a-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ec48a-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ec48a-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec48a-141">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
