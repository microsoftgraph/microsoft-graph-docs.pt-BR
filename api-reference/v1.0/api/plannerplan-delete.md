---
title: Excluir plannerPlan
description: Exclua **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 8abce6892ce981a9513570c1ba0d5a1a72c9724a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984702"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="82c16-103">Excluir plannerPlan</span><span class="sxs-lookup"><span data-stu-id="82c16-103">Delete plannerPlan</span></span>

<span data-ttu-id="82c16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82c16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82c16-105">Exclua **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="82c16-105">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="82c16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="82c16-106">Permissions</span></span>
<span data-ttu-id="82c16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82c16-109">Permission type</span></span>      | <span data-ttu-id="82c16-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82c16-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82c16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82c16-111">Delegated (work or school account)</span></span> | <span data-ttu-id="82c16-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c16-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82c16-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82c16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82c16-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c16-114">Not supported.</span></span>    |
|<span data-ttu-id="82c16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82c16-115">Application</span></span> | <span data-ttu-id="82c16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c16-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82c16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82c16-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/{id}

```
## <a name="request-headers"></a><span data-ttu-id="82c16-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82c16-118">Request headers</span></span>
| <span data-ttu-id="82c16-119">Nome</span><span class="sxs-lookup"><span data-stu-id="82c16-119">Name</span></span>       | <span data-ttu-id="82c16-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c16-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="82c16-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="82c16-121">Authorization</span></span>  | <span data-ttu-id="82c16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82c16-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82c16-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="82c16-124">If-Match</span></span>  | <span data-ttu-id="82c16-p103">O último valor ETag conhecido do objeto **plannerPlan** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82c16-p103">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82c16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82c16-127">Request body</span></span>
<span data-ttu-id="82c16-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82c16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82c16-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c16-129">Response</span></span>

<span data-ttu-id="82c16-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82c16-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="82c16-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="82c16-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="82c16-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82c16-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82c16-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82c16-136">Request</span></span>
<span data-ttu-id="82c16-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c16-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82c16-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="82c16-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/plans/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="c"></a>[<span data-ttu-id="82c16-139">C#</span><span class="sxs-lookup"><span data-stu-id="82c16-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82c16-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82c16-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82c16-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82c16-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82c16-142">Java</span><span class="sxs-lookup"><span data-stu-id="82c16-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82c16-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c16-143">Response</span></span>
<span data-ttu-id="82c16-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82c16-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

