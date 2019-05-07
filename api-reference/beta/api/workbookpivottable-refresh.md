---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 38d4f113040258823fdb4736e549399534fe35c6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636951"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="8a24c-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="8a24c-103">workbookPivotTable: refresh</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a24c-104">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="8a24c-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="8a24c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a24c-105">Permissions</span></span>
<span data-ttu-id="8a24c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8a24c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a24c-108">Permission type</span></span>      | <span data-ttu-id="8a24c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a24c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a24c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a24c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a24c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a24c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a24c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a24c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a24c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a24c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a24c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a24c-114">Application</span></span> | <span data-ttu-id="8a24c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a24c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a24c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a24c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="8a24c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a24c-117">Request headers</span></span>
| <span data-ttu-id="8a24c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8a24c-118">Name</span></span>       | <span data-ttu-id="8a24c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a24c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a24c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a24c-120">Authorization</span></span>  | <span data-ttu-id="8a24c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a24c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a24c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8a24c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8a24c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8a24c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a24c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a24c-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8a24c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a24c-127">Response</span></span>

<span data-ttu-id="8a24c-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a24c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a24c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a24c-130">Example</span></span>
<span data-ttu-id="8a24c-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8a24c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a24c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a24c-132">Request</span></span>
<span data-ttu-id="8a24c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a24c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="8a24c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a24c-134">Response</span></span>
<span data-ttu-id="8a24c-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a24c-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8a24c-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8a24c-136">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="8a24c-137">Basic</span><span class="sxs-lookup"><span data-stu-id="8a24c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookpivottable_refresh-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-refresh.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookpivottable-refresh.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
