---
title: Excluir plannerBucket
description: Exclua **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e9d941913d48bb56090bf3f271e768305398a5c6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595537"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="d8ef3-103">Excluir plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d8ef3-103">Delete plannerBucket</span></span>

<span data-ttu-id="d8ef3-104">Exclua **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-104">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8ef3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8ef3-105">Permissions</span></span>
<span data-ttu-id="d8ef3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ef3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8ef3-108">Permission type</span></span>      | <span data-ttu-id="d8ef3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8ef3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8ef3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8ef3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d8ef3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ef3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8ef3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8ef3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8ef3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-113">Not supported.</span></span>    |
|<span data-ttu-id="d8ef3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8ef3-114">Application</span></span> | <span data-ttu-id="d8ef3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8ef3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8ef3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d8ef3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ef3-117">Request headers</span></span>
| <span data-ttu-id="d8ef3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d8ef3-118">Name</span></span>       | <span data-ttu-id="d8ef3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8ef3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d8ef3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8ef3-120">Authorization</span></span>  | <span data-ttu-id="d8ef3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8ef3-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="d8ef3-123">If-Match</span></span>  | <span data-ttu-id="d8ef3-p103">O último valor ETag conhecido do objeto **plannerBucket** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ef3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ef3-126">Request body</span></span>
<span data-ttu-id="d8ef3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8ef3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ef3-128">Response</span></span>

<span data-ttu-id="d8ef3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="d8ef3-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d8ef3-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d8ef3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8ef3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8ef3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8ef3-135">Request</span></span>
<span data-ttu-id="d8ef3-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/buckets/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="d8ef3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8ef3-137">Response</span></span>
<span data-ttu-id="d8ef3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8ef3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8ef3-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d8ef3-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8ef3-142">Basic</span><span class="sxs-lookup"><span data-stu-id="d8ef3-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_plannerbucket-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8ef3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8ef3-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_plannerbucket-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerbucket-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerbucket-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
