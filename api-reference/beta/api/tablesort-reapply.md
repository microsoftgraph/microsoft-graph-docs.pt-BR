---
title: 'TableSort: reapply'
description: Reaplica os parâmetros de classificação atuais à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f3e8257aa4b37807fa37a0cc65e4091b7d5423af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452621"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="eb7d7-103">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="eb7d7-103">TableSort: reapply</span></span>

<span data-ttu-id="eb7d7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb7d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb7d7-105">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-105">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb7d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb7d7-106">Permissions</span></span>
<span data-ttu-id="eb7d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb7d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb7d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb7d7-109">Permission type</span></span>      | <span data-ttu-id="eb7d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb7d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb7d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb7d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb7d7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb7d7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb7d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb7d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb7d7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb7d7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb7d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb7d7-115">Application</span></span> | <span data-ttu-id="eb7d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb7d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb7d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="eb7d7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb7d7-118">Request headers</span></span>
| <span data-ttu-id="eb7d7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eb7d7-119">Name</span></span>       | <span data-ttu-id="eb7d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb7d7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb7d7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb7d7-121">Authorization</span></span>  | <span data-ttu-id="eb7d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb7d7-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eb7d7-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="eb7d7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb7d7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb7d7-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="eb7d7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb7d7-128">Response</span></span>

<span data-ttu-id="eb7d7-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb7d7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb7d7-131">Example</span></span>
<span data-ttu-id="eb7d7-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb7d7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb7d7-133">Request</span></span>
<span data-ttu-id="eb7d7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb7d7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb7d7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```
# <a name="c"></a>[<span data-ttu-id="eb7d7-136">C#</span><span class="sxs-lookup"><span data-stu-id="eb7d7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-reapply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb7d7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb7d7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-reapply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb7d7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb7d7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-reapply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eb7d7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb7d7-139">Response</span></span>
<span data-ttu-id="eb7d7-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb7d7-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
