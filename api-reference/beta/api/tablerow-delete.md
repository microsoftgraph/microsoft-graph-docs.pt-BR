---
title: 'TableRow: delete'
description: Exclui a linha da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e0a12f2160e1d3c9f35862c34fbe571ac2a8e3d7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452675"
---
# <a name="tablerow-delete"></a><span data-ttu-id="5a8e3-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="5a8e3-103">TableRow: delete</span></span>

<span data-ttu-id="5a8e3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5a8e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a8e3-105">Exclui a linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-105">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a8e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a8e3-106">Permissions</span></span>
<span data-ttu-id="5a8e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a8e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a8e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a8e3-109">Permission type</span></span>      | <span data-ttu-id="5a8e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a8e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a8e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a8e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5a8e3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a8e3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a8e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a8e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a8e3-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a8e3-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a8e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a8e3-115">Application</span></span> | <span data-ttu-id="5a8e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a8e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a8e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="5a8e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a8e3-118">Request headers</span></span>
| <span data-ttu-id="5a8e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5a8e3-119">Name</span></span>       | <span data-ttu-id="5a8e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a8e3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5a8e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a8e3-121">Authorization</span></span>  | <span data-ttu-id="5a8e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a8e3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5a8e3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5a8e3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a8e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a8e3-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5a8e3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a8e3-128">Response</span></span>

<span data-ttu-id="5a8e3-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a8e3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a8e3-131">Example</span></span>
<span data-ttu-id="5a8e3-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5a8e3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a8e3-133">Request</span></span>
<span data-ttu-id="5a8e3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="5a8e3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a8e3-135">Response</span></span>
<span data-ttu-id="5a8e3-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a8e3-136">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
