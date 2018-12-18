---
title: 'Range: unmerge'
description: Desfaz a mesclagem das células do intervalo em células separadas.
author: lumine2008
ms.openlocfilehash: 2b68ce5a034a274b1861d68db7a216cd797fa6c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334164"
---
# <a name="range-unmerge"></a><span data-ttu-id="4009e-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="4009e-103">Range: unmerge</span></span>

<span data-ttu-id="4009e-104">Desfaz a mesclagem das células do intervalo em células separadas.</span><span class="sxs-lookup"><span data-stu-id="4009e-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="4009e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4009e-105">Permissions</span></span>
<span data-ttu-id="4009e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4009e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4009e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4009e-108">Permission type</span></span>      | <span data-ttu-id="4009e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4009e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4009e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4009e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4009e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4009e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4009e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4009e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4009e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4009e-113">Not supported.</span></span>    |
|<span data-ttu-id="4009e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4009e-114">Application</span></span> | <span data-ttu-id="4009e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4009e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4009e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4009e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="4009e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4009e-117">Request headers</span></span>
| <span data-ttu-id="4009e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4009e-118">Name</span></span>       | <span data-ttu-id="4009e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4009e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4009e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4009e-120">Authorization</span></span>  | <span data-ttu-id="4009e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4009e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4009e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4009e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4009e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4009e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4009e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4009e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4009e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4009e-127">Response</span></span>

<span data-ttu-id="4009e-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4009e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4009e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4009e-130">Example</span></span>
<span data-ttu-id="4009e-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4009e-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4009e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4009e-132">Request</span></span>
<span data-ttu-id="4009e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4009e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```

##### <a name="response"></a><span data-ttu-id="4009e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4009e-134">Response</span></span>
<span data-ttu-id="4009e-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4009e-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->