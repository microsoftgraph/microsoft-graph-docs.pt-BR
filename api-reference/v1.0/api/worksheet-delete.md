---
title: 'Worksheet: delete'
description: Exclui a planilha da pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ee46051e611866c3e18d72396762276eb22f52e7
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515776"
---
# <a name="worksheet-delete"></a><span data-ttu-id="579f5-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="579f5-103">Worksheet: delete</span></span>

<span data-ttu-id="579f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="579f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="579f5-105">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="579f5-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="579f5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="579f5-106">Permissions</span></span>
<span data-ttu-id="579f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="579f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="579f5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="579f5-109">Permission type</span></span>      | <span data-ttu-id="579f5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="579f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="579f5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="579f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="579f5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="579f5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="579f5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="579f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="579f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="579f5-114">Not supported.</span></span>    |
|<span data-ttu-id="579f5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="579f5-115">Application</span></span> | <span data-ttu-id="579f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="579f5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="579f5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="579f5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /workbook/worksheets/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="579f5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="579f5-118">Request headers</span></span>
| <span data-ttu-id="579f5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="579f5-119">Name</span></span>       | <span data-ttu-id="579f5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="579f5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="579f5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="579f5-121">Authorization</span></span>  | <span data-ttu-id="579f5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="579f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="579f5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="579f5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="579f5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="579f5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="579f5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="579f5-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="579f5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="579f5-128">Response</span></span>

<span data-ttu-id="579f5-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="579f5-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="579f5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="579f5-131">Example</span></span>
<span data-ttu-id="579f5-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="579f5-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="579f5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="579f5-133">Request</span></span>
<span data-ttu-id="579f5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="579f5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
```

##### <a name="response"></a><span data-ttu-id="579f5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="579f5-135">Response</span></span>
<span data-ttu-id="579f5-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="579f5-136">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

