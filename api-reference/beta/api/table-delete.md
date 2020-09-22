---
title: 'Table: delete'
description: Exclui a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 234e9833a2f18b2060129958b59109fa025e9822
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087800"
---
# <a name="table-delete"></a><span data-ttu-id="e188b-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="e188b-103">Table: delete</span></span>

<span data-ttu-id="e188b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e188b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e188b-105">Exclui a tabela.</span><span class="sxs-lookup"><span data-stu-id="e188b-105">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="e188b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e188b-106">Permissions</span></span>
<span data-ttu-id="e188b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e188b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e188b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e188b-109">Permission type</span></span>      | <span data-ttu-id="e188b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e188b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e188b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e188b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e188b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e188b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e188b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e188b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e188b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e188b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e188b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e188b-115">Application</span></span> | <span data-ttu-id="e188b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e188b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e188b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e188b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="e188b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e188b-118">Request headers</span></span>
| <span data-ttu-id="e188b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e188b-119">Name</span></span>       | <span data-ttu-id="e188b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e188b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e188b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e188b-121">Authorization</span></span>  | <span data-ttu-id="e188b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e188b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e188b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e188b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e188b-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e188b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e188b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e188b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e188b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e188b-128">Response</span></span>

<span data-ttu-id="e188b-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e188b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e188b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e188b-131">Example</span></span>
<span data-ttu-id="e188b-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e188b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e188b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e188b-133">Request</span></span>
<span data-ttu-id="e188b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e188b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="e188b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e188b-135">Response</span></span>
<span data-ttu-id="e188b-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e188b-136">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


