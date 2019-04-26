---
title: 'ChartFill: setSolidColor'
description: Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c26bea1300819ea388be8b250468bcf54dc15b59
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327768"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="7665d-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="7665d-103">ChartFill: setSolidColor</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7665d-104">Define a formatação de preenchimento de um elemento do gráfico com uma cor uniforme.</span><span class="sxs-lookup"><span data-stu-id="7665d-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="7665d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7665d-105">Permissions</span></span>
<span data-ttu-id="7665d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7665d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7665d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7665d-108">Permission type</span></span>      | <span data-ttu-id="7665d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7665d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7665d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7665d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7665d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7665d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7665d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7665d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7665d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7665d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7665d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7665d-114">Application</span></span> | <span data-ttu-id="7665d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7665d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7665d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7665d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="7665d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7665d-117">Request headers</span></span>
| <span data-ttu-id="7665d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7665d-118">Name</span></span>       | <span data-ttu-id="7665d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7665d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7665d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7665d-120">Authorization</span></span>  | <span data-ttu-id="7665d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7665d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7665d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7665d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7665d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7665d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7665d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7665d-126">Request body</span></span>
<span data-ttu-id="7665d-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7665d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7665d-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7665d-128">Parameter</span></span>    | <span data-ttu-id="7665d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7665d-129">Type</span></span>   |<span data-ttu-id="7665d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7665d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7665d-131">color</span><span class="sxs-lookup"><span data-stu-id="7665d-131">color</span></span>|<span data-ttu-id="7665d-132">string</span><span class="sxs-lookup"><span data-stu-id="7665d-132">string</span></span>|<span data-ttu-id="7665d-133">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="7665d-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="7665d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7665d-134">Response</span></span>

<span data-ttu-id="7665d-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7665d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7665d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7665d-137">Example</span></span>
<span data-ttu-id="7665d-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7665d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7665d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7665d-139">Request</span></span>
<span data-ttu-id="7665d-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7665d-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="7665d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7665d-141">Response</span></span>
<span data-ttu-id="7665d-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7665d-142">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
