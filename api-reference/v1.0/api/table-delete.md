---
title: 'Table: delete'
description: Exclui a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 06c0d91008805ef2efc33cecc3f0bccef13fcf03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970947"
---
# <a name="table-delete"></a><span data-ttu-id="5fd64-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="5fd64-103">Table: delete</span></span>

<span data-ttu-id="5fd64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fd64-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fd64-105">Exclui a tabela.</span><span class="sxs-lookup"><span data-stu-id="5fd64-105">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5fd64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fd64-106">Permissions</span></span>
<span data-ttu-id="5fd64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fd64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fd64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fd64-109">Permission type</span></span>      | <span data-ttu-id="5fd64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fd64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fd64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fd64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5fd64-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5fd64-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5fd64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fd64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fd64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fd64-114">Not supported.</span></span>    |
|<span data-ttu-id="5fd64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fd64-115">Application</span></span> | <span data-ttu-id="5fd64-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fd64-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fd64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fd64-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="5fd64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd64-118">Request headers</span></span>
| <span data-ttu-id="5fd64-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5fd64-119">Name</span></span>       | <span data-ttu-id="5fd64-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fd64-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5fd64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fd64-121">Authorization</span></span>  | <span data-ttu-id="5fd64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fd64-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fd64-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5fd64-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5fd64-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5fd64-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fd64-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd64-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5fd64-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fd64-128">Response</span></span>

<span data-ttu-id="5fd64-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fd64-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fd64-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fd64-131">Example</span></span>
<span data-ttu-id="5fd64-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5fd64-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5fd64-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd64-133">Request</span></span>
<span data-ttu-id="5fd64-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fd64-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="5fd64-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fd64-135">Response</span></span>
<span data-ttu-id="5fd64-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fd64-136">Here is an example of the response.</span></span> 
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

