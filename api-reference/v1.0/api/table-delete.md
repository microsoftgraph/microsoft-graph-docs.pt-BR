---
title: 'Table: delete'
description: Exclui a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 92c75c3297c7d3f2d43961aff4e82710834d35e3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516672"
---
# <a name="table-delete"></a><span data-ttu-id="e1949-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="e1949-103">Table: delete</span></span>

<span data-ttu-id="e1949-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1949-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1949-105">Exclui a tabela.</span><span class="sxs-lookup"><span data-stu-id="e1949-105">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1949-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1949-106">Permissions</span></span>
<span data-ttu-id="e1949-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1949-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1949-109">Permission type</span></span>      | <span data-ttu-id="e1949-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1949-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1949-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1949-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1949-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1949-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e1949-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1949-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1949-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1949-114">Not supported.</span></span>    |
|<span data-ttu-id="e1949-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1949-115">Application</span></span> | <span data-ttu-id="e1949-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1949-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1949-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1949-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /workbook/tables/{id|name}
DELETE /workbook/worksheets/{id|name}/tables/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="e1949-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1949-118">Request headers</span></span>
| <span data-ttu-id="e1949-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e1949-119">Name</span></span>       | <span data-ttu-id="e1949-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1949-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1949-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1949-121">Authorization</span></span>  | <span data-ttu-id="e1949-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1949-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1949-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e1949-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e1949-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1949-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1949-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1949-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e1949-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1949-128">Response</span></span>

<span data-ttu-id="e1949-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1949-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1949-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1949-131">Example</span></span>
<span data-ttu-id="e1949-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e1949-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e1949-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1949-133">Request</span></span>
<span data-ttu-id="e1949-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1949-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
```

##### <a name="response"></a><span data-ttu-id="e1949-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1949-135">Response</span></span>
<span data-ttu-id="e1949-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1949-136">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

