---
title: 'TableColumn: delete'
description: Exclui a coluna da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 536e2b5f1672f2e7c75603b8fb2d70308e2c0bcb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509595"
---
# <a name="tablecolumn-delete"></a><span data-ttu-id="f4deb-103">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="f4deb-103">TableColumn: delete</span></span>

<span data-ttu-id="f4deb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4deb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4deb-105">Exclui a coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="f4deb-105">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4deb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4deb-106">Permissions</span></span>
<span data-ttu-id="f4deb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4deb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4deb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4deb-109">Permission type</span></span>      | <span data-ttu-id="f4deb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4deb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4deb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4deb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4deb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4deb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f4deb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4deb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4deb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4deb-114">Not supported.</span></span>    |
|<span data-ttu-id="f4deb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4deb-115">Application</span></span> | <span data-ttu-id="f4deb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4deb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4deb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4deb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="f4deb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4deb-118">Request headers</span></span>
| <span data-ttu-id="f4deb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f4deb-119">Name</span></span>       | <span data-ttu-id="f4deb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4deb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4deb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4deb-121">Authorization</span></span>  | <span data-ttu-id="f4deb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4deb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4deb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f4deb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f4deb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f4deb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4deb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4deb-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f4deb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4deb-128">Response</span></span>

<span data-ttu-id="f4deb-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4deb-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4deb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4deb-131">Example</span></span>
<span data-ttu-id="f4deb-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f4deb-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f4deb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4deb-133">Request</span></span>
<span data-ttu-id="f4deb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4deb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="f4deb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4deb-135">Response</span></span>
<span data-ttu-id="f4deb-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4deb-136">Here is an example of the response.</span></span> 
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
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
