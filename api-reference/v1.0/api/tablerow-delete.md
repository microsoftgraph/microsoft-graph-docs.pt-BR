---
title: 'TableRow: delete'
description: Exclui a linha da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f8b9139ac4eed6c2acbd68063ddb2b10021196fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024354"
---
# <a name="tablerow-delete"></a><span data-ttu-id="9782a-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="9782a-103">TableRow: delete</span></span>

<span data-ttu-id="9782a-104">Exclui a linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="9782a-104">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9782a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9782a-105">Permissions</span></span>
<span data-ttu-id="9782a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9782a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9782a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9782a-108">Permission type</span></span>      | <span data-ttu-id="9782a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9782a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9782a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9782a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9782a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9782a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9782a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9782a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9782a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9782a-113">Not supported.</span></span>    |
|<span data-ttu-id="9782a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9782a-114">Application</span></span> | <span data-ttu-id="9782a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9782a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9782a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9782a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="9782a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9782a-117">Request headers</span></span>
| <span data-ttu-id="9782a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9782a-118">Name</span></span>       | <span data-ttu-id="9782a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9782a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9782a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9782a-120">Authorization</span></span>  | <span data-ttu-id="9782a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9782a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9782a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9782a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9782a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9782a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9782a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9782a-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9782a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9782a-127">Response</span></span>

<span data-ttu-id="9782a-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9782a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9782a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9782a-130">Example</span></span>
<span data-ttu-id="9782a-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9782a-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9782a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9782a-132">Request</span></span>
<span data-ttu-id="9782a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9782a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="9782a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9782a-134">Response</span></span>
<span data-ttu-id="9782a-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9782a-135">Here is an example of the response.</span></span> 
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
