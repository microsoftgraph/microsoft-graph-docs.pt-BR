---
title: 'TableColumn: delete'
description: Exclui a coluna da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2154bbb7a28d34b08ec1e8cbfa0f6ca3fa14f1ef
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578336"
---
# <a name="tablecolumn-delete"></a><span data-ttu-id="f5bae-103">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="f5bae-103">TableColumn: delete</span></span>

<span data-ttu-id="f5bae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5bae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5bae-105">Exclui a coluna da tabela.</span><span class="sxs-lookup"><span data-stu-id="f5bae-105">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5bae-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5bae-106">Permissions</span></span>
<span data-ttu-id="f5bae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5bae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5bae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5bae-109">Permission type</span></span>      | <span data-ttu-id="f5bae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5bae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5bae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5bae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f5bae-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5bae-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5bae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5bae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5bae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5bae-114">Not supported.</span></span>    |
|<span data-ttu-id="f5bae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5bae-115">Application</span></span> | <span data-ttu-id="f5bae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5bae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5bae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5bae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="f5bae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5bae-118">Request headers</span></span>
| <span data-ttu-id="f5bae-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f5bae-119">Name</span></span>       | <span data-ttu-id="f5bae-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5bae-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5bae-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5bae-121">Authorization</span></span>  | <span data-ttu-id="f5bae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5bae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5bae-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f5bae-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5bae-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f5bae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5bae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5bae-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f5bae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5bae-128">Response</span></span>

<span data-ttu-id="f5bae-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5bae-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5bae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5bae-131">Example</span></span>
<span data-ttu-id="f5bae-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f5bae-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5bae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5bae-133">Request</span></span>
<span data-ttu-id="f5bae-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5bae-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```

##### <a name="response"></a><span data-ttu-id="f5bae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5bae-135">Response</span></span>
<span data-ttu-id="f5bae-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5bae-136">Here is an example of the response.</span></span> 
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

