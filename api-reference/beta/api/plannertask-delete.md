---
title: Excluir plannerTask
description: Exclua **plannerTask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9864924f91c6120cb7998587600c95f5c732f0e4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264334"
---
# <a name="delete-plannertask"></a><span data-ttu-id="f1e2f-103">Excluir plannerTask</span><span class="sxs-lookup"><span data-stu-id="f1e2f-103">Delete plannerTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1e2f-104">Exclua **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-104">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1e2f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1e2f-105">Permissions</span></span>
<span data-ttu-id="f1e2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e2f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1e2f-108">Permission type</span></span>      | <span data-ttu-id="f1e2f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1e2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1e2f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1e2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1e2f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e2f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1e2f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1e2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1e2f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-113">Not supported.</span></span>    |
|<span data-ttu-id="f1e2f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1e2f-114">Application</span></span> | <span data-ttu-id="f1e2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1e2f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1e2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/<id>
```
## <a name="request-headers"></a><span data-ttu-id="f1e2f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e2f-117">Request headers</span></span>
| <span data-ttu-id="f1e2f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f1e2f-118">Name</span></span>       | <span data-ttu-id="f1e2f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1e2f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1e2f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1e2f-120">Authorization</span></span>  | <span data-ttu-id="f1e2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1e2f-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="f1e2f-123">If-Match</span></span>  | <span data-ttu-id="f1e2f-p103">O último valor ETag conhecido do objeto **plannerTask** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e2f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e2f-126">Request body</span></span>
<span data-ttu-id="f1e2f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1e2f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e2f-128">Response</span></span>

<span data-ttu-id="f1e2f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f1e2f-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f1e2f-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f1e2f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1e2f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1e2f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e2f-135">Request</span></span>
<span data-ttu-id="f1e2f-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/tasks/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="f1e2f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e2f-137">Response</span></span>
<span data-ttu-id="f1e2f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1e2f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1e2f-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f1e2f-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1e2f-142">C#</span><span class="sxs-lookup"><span data-stu-id="f1e2f-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_plannertask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1e2f-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1e2f-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_plannertask-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1e2f-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f1e2f-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_plannertask-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/plannertask-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannertask-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannertask-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
