---
title: 'Chart: setPosition'
description: Posiciona o gráfico em relação às células na planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d8e4c65954790fcebc885a84183b7941e2701e28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981809"
---
# <a name="chart-setposition"></a><span data-ttu-id="caf2c-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="caf2c-103">Chart: setPosition</span></span>

<span data-ttu-id="caf2c-104">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="caf2c-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="caf2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="caf2c-105">Permissions</span></span>
<span data-ttu-id="caf2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caf2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caf2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caf2c-108">Permission type</span></span>      | <span data-ttu-id="caf2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="caf2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caf2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caf2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="caf2c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caf2c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="caf2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caf2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf2c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caf2c-113">Not supported.</span></span>    |
|<span data-ttu-id="caf2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caf2c-114">Application</span></span> | <span data-ttu-id="caf2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caf2c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="caf2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caf2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="caf2c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caf2c-117">Request headers</span></span>
| <span data-ttu-id="caf2c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="caf2c-118">Name</span></span>       | <span data-ttu-id="caf2c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="caf2c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="caf2c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="caf2c-120">Authorization</span></span>  | <span data-ttu-id="caf2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caf2c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="caf2c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="caf2c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="caf2c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="caf2c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="caf2c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caf2c-126">Request body</span></span>
<span data-ttu-id="caf2c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="caf2c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="caf2c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="caf2c-128">Parameter</span></span>    | <span data-ttu-id="caf2c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="caf2c-129">Type</span></span>   |<span data-ttu-id="caf2c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="caf2c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caf2c-131">startCell</span><span class="sxs-lookup"><span data-stu-id="caf2c-131">startCell</span></span>|<span data-ttu-id="caf2c-132">Json</span><span class="sxs-lookup"><span data-stu-id="caf2c-132">Json</span></span>|<span data-ttu-id="caf2c-p104">A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.</span><span class="sxs-lookup"><span data-stu-id="caf2c-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="caf2c-136">endCell</span><span class="sxs-lookup"><span data-stu-id="caf2c-136">endCell</span></span>|<span data-ttu-id="caf2c-137">Json</span><span class="sxs-lookup"><span data-stu-id="caf2c-137">Json</span></span>|<span data-ttu-id="caf2c-p105">Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.</span><span class="sxs-lookup"><span data-stu-id="caf2c-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="caf2c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="caf2c-141">Response</span></span>

<span data-ttu-id="caf2c-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caf2c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caf2c-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caf2c-144">Example</span></span>
<span data-ttu-id="caf2c-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="caf2c-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="caf2c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caf2c-146">Request</span></span>
<span data-ttu-id="caf2c-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="caf2c-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="caf2c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="caf2c-148">Response</span></span>
<span data-ttu-id="caf2c-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caf2c-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
