---
title: Excluir plannerTask
description: Exclua **plannerTask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 90fa423a961a95e8407232bf5540baf69343f17e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966825"
---
# <a name="delete-plannertask"></a><span data-ttu-id="59226-103">Excluir plannerTask</span><span class="sxs-lookup"><span data-stu-id="59226-103">Delete plannerTask</span></span>

<span data-ttu-id="59226-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59226-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59226-105">Exclua **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="59226-105">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="59226-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59226-106">Permissions</span></span>
<span data-ttu-id="59226-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59226-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59226-109">Permission type</span></span>      | <span data-ttu-id="59226-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59226-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59226-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59226-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59226-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59226-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="59226-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59226-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59226-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59226-114">Not supported.</span></span>    |
|<span data-ttu-id="59226-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59226-115">Application</span></span> | <span data-ttu-id="59226-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59226-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59226-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59226-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59226-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59226-118">Request headers</span></span>
| <span data-ttu-id="59226-119">Nome</span><span class="sxs-lookup"><span data-stu-id="59226-119">Name</span></span>       | <span data-ttu-id="59226-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="59226-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59226-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59226-121">Authorization</span></span>  | <span data-ttu-id="59226-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59226-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59226-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="59226-124">If-Match</span></span>  | <span data-ttu-id="59226-p103">O último valor ETag conhecido do objeto **plannerTask** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59226-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59226-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59226-127">Request body</span></span>
<span data-ttu-id="59226-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59226-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59226-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="59226-129">Response</span></span>

<span data-ttu-id="59226-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59226-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="59226-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="59226-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="59226-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59226-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59226-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59226-136">Request</span></span>
<span data-ttu-id="59226-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59226-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59226-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="59226-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/tasks/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="c"></a>[<span data-ttu-id="59226-139">C#</span><span class="sxs-lookup"><span data-stu-id="59226-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59226-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59226-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59226-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59226-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59226-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="59226-142">Response</span></span>
<span data-ttu-id="59226-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59226-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


