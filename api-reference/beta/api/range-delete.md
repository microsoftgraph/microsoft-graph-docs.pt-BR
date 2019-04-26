---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 59531c4a4d8fa3abcb3a857cbaca4487299b8d6e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337026"
---
# <a name="range-delete"></a><span data-ttu-id="bdeea-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="bdeea-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdeea-104">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="bdeea-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="bdeea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdeea-105">Permissions</span></span>
<span data-ttu-id="bdeea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdeea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdeea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdeea-108">Permission type</span></span>      | <span data-ttu-id="bdeea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdeea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdeea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdeea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdeea-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdeea-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdeea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdeea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdeea-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdeea-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdeea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdeea-114">Application</span></span> | <span data-ttu-id="bdeea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdeea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdeea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdeea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="bdeea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdeea-117">Request headers</span></span>
| <span data-ttu-id="bdeea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bdeea-118">Name</span></span>       | <span data-ttu-id="bdeea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdeea-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bdeea-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdeea-120">Authorization</span></span>  | <span data-ttu-id="bdeea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdeea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdeea-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bdeea-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bdeea-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bdeea-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdeea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdeea-126">Request body</span></span>
<span data-ttu-id="bdeea-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdeea-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bdeea-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bdeea-128">Parameter</span></span>    | <span data-ttu-id="bdeea-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdeea-129">Type</span></span>   |<span data-ttu-id="bdeea-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdeea-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdeea-131">shift</span><span class="sxs-lookup"><span data-stu-id="bdeea-131">shift</span></span>|<span data-ttu-id="bdeea-132">string</span><span class="sxs-lookup"><span data-stu-id="bdeea-132">string</span></span>|<span data-ttu-id="bdeea-p104">Especifica como deslocar as células.  Os valores possíveis são: `Up` e `Left`.</span><span class="sxs-lookup"><span data-stu-id="bdeea-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="bdeea-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdeea-135">Response</span></span>

<span data-ttu-id="bdeea-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdeea-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdeea-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdeea-138">Example</span></span>
<span data-ttu-id="bdeea-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bdeea-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bdeea-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdeea-140">Request</span></span>
<span data-ttu-id="bdeea-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdeea-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="bdeea-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdeea-142">Response</span></span>
<span data-ttu-id="bdeea-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdeea-143">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
