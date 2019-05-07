---
title: 'Table: clearFilters'
description: Limpa todos os filtros aplicados à tabela no momento.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1a35b103c01e0ad6a46be39a4231de63e3dae337
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637896"
---
# <a name="table-clearfilters"></a><span data-ttu-id="fd322-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="fd322-103">Table: clearFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd322-104">Limpa todos os filtros aplicados à tabela no momento.</span><span class="sxs-lookup"><span data-stu-id="fd322-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd322-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd322-105">Permissions</span></span>
<span data-ttu-id="fd322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd322-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd322-108">Permission type</span></span>      | <span data-ttu-id="fd322-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd322-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd322-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd322-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd322-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd322-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd322-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd322-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd322-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd322-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd322-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd322-114">Application</span></span> | <span data-ttu-id="fd322-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd322-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd322-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd322-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="fd322-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd322-117">Request headers</span></span>
| <span data-ttu-id="fd322-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fd322-118">Name</span></span>       | <span data-ttu-id="fd322-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd322-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd322-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd322-120">Authorization</span></span>  | <span data-ttu-id="fd322-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd322-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd322-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fd322-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fd322-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fd322-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd322-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd322-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fd322-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd322-127">Response</span></span>

<span data-ttu-id="fd322-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd322-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd322-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd322-130">Example</span></span>
<span data-ttu-id="fd322-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fd322-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd322-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd322-132">Request</span></span>
<span data-ttu-id="fd322-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd322-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="fd322-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd322-134">Response</span></span>
<span data-ttu-id="fd322-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd322-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd322-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fd322-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd322-137">Basic</span><span class="sxs-lookup"><span data-stu-id="fd322-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_clearfilters-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd322-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd322-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_clearfilters-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-clearfilters.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-clearfilters.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
