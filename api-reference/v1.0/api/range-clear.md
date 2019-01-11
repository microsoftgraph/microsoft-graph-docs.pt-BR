---
title: 'Range: clear'
description: Limpa valores de intervalo, formatação, preenchimento, borda, etc.
localization_priority: Normal
ms.openlocfilehash: 8bf7bafd42947528c98a83819afd7b16f49d2e7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861912"
---
# <a name="range-clear"></a><span data-ttu-id="f3307-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="f3307-103">Range: clear</span></span>

<span data-ttu-id="f3307-104">Limpa valores de intervalo, formatação, preenchimento, borda, etc.</span><span class="sxs-lookup"><span data-stu-id="f3307-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3307-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3307-105">Permissions</span></span>
<span data-ttu-id="f3307-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3307-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3307-108">Permission type</span></span>      | <span data-ttu-id="f3307-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3307-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3307-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3307-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3307-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3307-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3307-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3307-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3307-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3307-113">Not supported.</span></span>    |
|<span data-ttu-id="f3307-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3307-114">Application</span></span> | <span data-ttu-id="f3307-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3307-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3307-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3307-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="f3307-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3307-117">Request headers</span></span>
| <span data-ttu-id="f3307-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f3307-118">Name</span></span>       | <span data-ttu-id="f3307-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3307-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3307-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3307-120">Authorization</span></span>  | <span data-ttu-id="f3307-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3307-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3307-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3307-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3307-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3307-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3307-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3307-126">Request body</span></span>
<span data-ttu-id="f3307-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3307-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3307-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f3307-128">Parameter</span></span>    | <span data-ttu-id="f3307-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3307-129">Type</span></span>   |<span data-ttu-id="f3307-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3307-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3307-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="f3307-131">applyTo</span></span>|<span data-ttu-id="f3307-132">string</span><span class="sxs-lookup"><span data-stu-id="f3307-132">string</span></span>|<span data-ttu-id="f3307-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f3307-133">Optional.</span></span> <span data-ttu-id="f3307-134">Determina o tipo de ação clara.</span><span class="sxs-lookup"><span data-stu-id="f3307-134">Determines the type of clear action.</span></span>  <span data-ttu-id="f3307-135">Os valores possíveis são: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="f3307-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="f3307-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3307-136">Response</span></span>

<span data-ttu-id="f3307-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3307-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3307-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3307-139">Example</span></span>
<span data-ttu-id="f3307-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f3307-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3307-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3307-141">Request</span></span>
<span data-ttu-id="f3307-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3307-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="f3307-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3307-143">Response</span></span>
<span data-ttu-id="f3307-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3307-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
