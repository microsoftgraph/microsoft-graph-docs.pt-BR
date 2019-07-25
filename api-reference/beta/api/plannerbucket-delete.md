---
title: Excluir plannerBucket
description: Exclua **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 286514d878be65638b267369ff70073c8c736b77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876593"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="072d0-103">Excluir plannerBucket</span><span class="sxs-lookup"><span data-stu-id="072d0-103">Delete plannerBucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="072d0-104">Exclua **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="072d0-104">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="072d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="072d0-105">Permissions</span></span>
<span data-ttu-id="072d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="072d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="072d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="072d0-108">Permission type</span></span>      | <span data-ttu-id="072d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="072d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="072d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="072d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="072d0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="072d0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="072d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="072d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="072d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="072d0-113">Not supported.</span></span>    |
|<span data-ttu-id="072d0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="072d0-114">Application</span></span> | <span data-ttu-id="072d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="072d0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="072d0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="072d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/<id>
```
## <a name="request-headers"></a><span data-ttu-id="072d0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="072d0-117">Request headers</span></span>
| <span data-ttu-id="072d0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="072d0-118">Name</span></span>       | <span data-ttu-id="072d0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="072d0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="072d0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="072d0-120">Authorization</span></span>  | <span data-ttu-id="072d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="072d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="072d0-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="072d0-123">If-Match</span></span>  | <span data-ttu-id="072d0-p103">O último valor ETag conhecido do objeto **plannerBucket** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="072d0-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="072d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="072d0-126">Request body</span></span>
<span data-ttu-id="072d0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="072d0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="072d0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="072d0-128">Response</span></span>

<span data-ttu-id="072d0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="072d0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="072d0-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="072d0-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="072d0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="072d0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="072d0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="072d0-135">Request</span></span>
<span data-ttu-id="072d0-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="072d0-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="072d0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="072d0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/buckets/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="072d0-138">C#</span><span class="sxs-lookup"><span data-stu-id="072d0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="072d0-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="072d0-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="072d0-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="072d0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="072d0-141">Java</span><span class="sxs-lookup"><span data-stu-id="072d0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="072d0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="072d0-142">Response</span></span>
<span data-ttu-id="072d0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="072d0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
