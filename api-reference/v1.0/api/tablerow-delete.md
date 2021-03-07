---
title: 'TableRow: delete'
description: Exclui a linha da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c98aa15c2e969d760a266842fe03d4a679757dc2
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516546"
---
# <a name="tablerow-delete"></a><span data-ttu-id="51015-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="51015-103">TableRow: delete</span></span>

<span data-ttu-id="51015-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51015-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51015-105">Exclui a linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="51015-105">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="51015-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="51015-106">Permissions</span></span>
<span data-ttu-id="51015-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51015-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51015-109">Permission type</span></span>      | <span data-ttu-id="51015-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51015-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51015-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51015-111">Delegated (work or school account)</span></span> | <span data-ttu-id="51015-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51015-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="51015-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51015-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51015-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51015-114">Not supported.</span></span>    |
|<span data-ttu-id="51015-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51015-115">Application</span></span> | <span data-ttu-id="51015-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51015-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51015-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51015-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /workbook/tables/{id|name}/rows/{index}
DELETE /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}

```
## <a name="request-headers"></a><span data-ttu-id="51015-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51015-118">Request headers</span></span>
| <span data-ttu-id="51015-119">Nome</span><span class="sxs-lookup"><span data-stu-id="51015-119">Name</span></span>       | <span data-ttu-id="51015-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="51015-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51015-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="51015-121">Authorization</span></span>  | <span data-ttu-id="51015-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51015-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51015-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="51015-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="51015-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="51015-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51015-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51015-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="51015-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="51015-128">Response</span></span>

<span data-ttu-id="51015-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51015-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51015-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51015-131">Example</span></span>
<span data-ttu-id="51015-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="51015-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51015-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51015-133">Request</span></span>
<span data-ttu-id="51015-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51015-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```

##### <a name="response"></a><span data-ttu-id="51015-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="51015-135">Response</span></span>
<span data-ttu-id="51015-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51015-136">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

