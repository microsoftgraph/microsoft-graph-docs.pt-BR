---
title: 'Chart: setPosition'
description: Posiciona o gráfico em relação às células na planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dae44414db5a095c4cf12506582a9533972a0373
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941216"
---
# <a name="chart-setposition"></a><span data-ttu-id="90587-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="90587-103">Chart: setPosition</span></span>

> <span data-ttu-id="90587-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90587-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90587-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90587-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90587-106">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="90587-106">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="90587-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90587-107">Permissions</span></span>
<span data-ttu-id="90587-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90587-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90587-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90587-110">Permission type</span></span>      | <span data-ttu-id="90587-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90587-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90587-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90587-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90587-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90587-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90587-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90587-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90587-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90587-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90587-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90587-116">Application</span></span> | <span data-ttu-id="90587-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90587-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90587-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90587-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="90587-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90587-119">Request headers</span></span>
| <span data-ttu-id="90587-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90587-120">Name</span></span>       | <span data-ttu-id="90587-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="90587-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90587-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90587-122">Authorization</span></span>  | <span data-ttu-id="90587-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90587-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90587-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90587-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="90587-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="90587-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90587-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90587-128">Request body</span></span>
<span data-ttu-id="90587-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90587-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90587-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="90587-130">Parameter</span></span>    | <span data-ttu-id="90587-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90587-131">Type</span></span>   |<span data-ttu-id="90587-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90587-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90587-133">startCell</span><span class="sxs-lookup"><span data-stu-id="90587-133">startCell</span></span>|<span data-ttu-id="90587-134">string</span><span class="sxs-lookup"><span data-stu-id="90587-134">string</span></span>|<span data-ttu-id="90587-p105">A célula inicial. Esse é o local para o qual o gráfico será movido. A célula inicial é a célula superior esquerda ou direita, dependendo das configurações de exibição do usuário, da esquerda para a direita.</span><span class="sxs-lookup"><span data-stu-id="90587-p105">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="90587-138">endCell</span><span class="sxs-lookup"><span data-stu-id="90587-138">endCell</span></span>|<span data-ttu-id="90587-139">string</span><span class="sxs-lookup"><span data-stu-id="90587-139">string</span></span>|<span data-ttu-id="90587-p106">Opcional. A célula final. Quando é especificada, a altura e a largura do gráfico são definidas para cobrirem totalmente essa célula ou intervalo.</span><span class="sxs-lookup"><span data-stu-id="90587-p106">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="90587-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="90587-143">Response</span></span>

<span data-ttu-id="90587-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90587-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90587-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90587-146">Example</span></span>
<span data-ttu-id="90587-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="90587-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="90587-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90587-148">Request</span></span>
<span data-ttu-id="90587-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90587-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="90587-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="90587-150">Response</span></span>
<span data-ttu-id="90587-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90587-151">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
