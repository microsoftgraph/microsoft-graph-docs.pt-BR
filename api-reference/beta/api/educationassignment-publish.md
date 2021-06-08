---
title: 'educationAssignment: publish'
description: Essa ação altera o estado de uma atribuição de seu status de rascunho original para o status publicado. Somente um professor da classe pode fazer essa chamada. Quando uma atribuição estiver no status de rascunho, os alunos não verão a atribuição, nem haverá objetos de envio. Quando você chama essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ac840109209b2a8ec5081d55abc31e1fac92d965
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785995"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="4ed4a-106">educationAssignment: publish</span><span class="sxs-lookup"><span data-stu-id="4ed4a-106">educationAssignment: publish</span></span>

<span data-ttu-id="4ed4a-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ed4a-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ed4a-108">Essa ação altera o estado de uma atribuição de seu status de rascunho original para o status publicado.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="4ed4a-109">Somente um professor da classe pode fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="4ed4a-110">Quando uma atribuição estiver no status de rascunho, os alunos não verão a atribuição, nem haverá objetos de envio.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="4ed4a-111">Quando você chama essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ed4a-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ed4a-112">Permissions</span></span>
<span data-ttu-id="4ed4a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ed4a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed4a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ed4a-115">Permission type</span></span>      | <span data-ttu-id="4ed4a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ed4a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ed4a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ed4a-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="4ed4a-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ed4a-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4ed4a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ed4a-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4ed4a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-120">Not supported.</span></span>  |
|<span data-ttu-id="4ed4a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ed4a-121">Application</span></span> | <span data-ttu-id="4ed4a-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4ed4a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed4a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="4ed4a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed4a-124">Request headers</span></span>
| <span data-ttu-id="4ed4a-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ed4a-125">Header</span></span>       | <span data-ttu-id="4ed4a-126">Valor</span><span class="sxs-lookup"><span data-stu-id="4ed4a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ed4a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ed4a-127">Authorization</span></span>  | <span data-ttu-id="4ed4a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ed4a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed4a-130">Request body</span></span>
<span data-ttu-id="4ed4a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ed4a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed4a-132">Response</span></span>
<span data-ttu-id="4ed4a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed4a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ed4a-135">Example</span></span>
<span data-ttu-id="4ed4a-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ed4a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed4a-137">Request</span></span>
<span data-ttu-id="4ed4a-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ed4a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed4a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="4ed4a-140">C#</span><span class="sxs-lookup"><span data-stu-id="4ed4a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ed4a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ed4a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ed4a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ed4a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ed4a-143">Java</span><span class="sxs-lookup"><span data-stu-id="4ed4a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ed4a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed4a-144">Response</span></span>
<span data-ttu-id="4ed4a-145">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="4ed4a-145">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


