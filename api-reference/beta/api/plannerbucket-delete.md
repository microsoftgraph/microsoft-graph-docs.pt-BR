---
title: Excluir plannerBucket
description: Exclua **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f3d22f773b28209c44512683bee56e26df8fb82c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971631"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="00a17-103">Excluir plannerBucket</span><span class="sxs-lookup"><span data-stu-id="00a17-103">Delete plannerBucket</span></span>

<span data-ttu-id="00a17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00a17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00a17-105">Exclua **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="00a17-105">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="00a17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00a17-106">Permissions</span></span>
<span data-ttu-id="00a17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00a17-109">Permission type</span></span>      | <span data-ttu-id="00a17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00a17-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00a17-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00a17-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00a17-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a17-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="00a17-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00a17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00a17-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00a17-114">Not supported.</span></span>    |
|<span data-ttu-id="00a17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00a17-115">Application</span></span> | <span data-ttu-id="00a17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00a17-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00a17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00a17-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00a17-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00a17-118">Request headers</span></span>
| <span data-ttu-id="00a17-119">Nome</span><span class="sxs-lookup"><span data-stu-id="00a17-119">Name</span></span>       | <span data-ttu-id="00a17-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="00a17-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00a17-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="00a17-121">Authorization</span></span>  | <span data-ttu-id="00a17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00a17-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00a17-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="00a17-124">If-Match</span></span>  | <span data-ttu-id="00a17-p103">O último valor ETag conhecido do objeto **plannerBucket** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00a17-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a17-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00a17-127">Request body</span></span>
<span data-ttu-id="00a17-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00a17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00a17-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="00a17-129">Response</span></span>

<span data-ttu-id="00a17-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00a17-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="00a17-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="00a17-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="00a17-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00a17-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00a17-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00a17-136">Request</span></span>
<span data-ttu-id="00a17-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00a17-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00a17-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="00a17-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/buckets/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="c"></a>[<span data-ttu-id="00a17-139">C#</span><span class="sxs-lookup"><span data-stu-id="00a17-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00a17-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00a17-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00a17-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00a17-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00a17-142">Java</span><span class="sxs-lookup"><span data-stu-id="00a17-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="00a17-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="00a17-143">Response</span></span>
<span data-ttu-id="00a17-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00a17-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


