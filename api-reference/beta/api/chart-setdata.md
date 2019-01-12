---
title: 'Chart: setData'
description: Redefine os dados de origem do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a92fe8e0c43b5dff4a406efbe0c2238ff0cab0ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921658"
---
# <a name="chart-setdata"></a><span data-ttu-id="01e48-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="01e48-103">Chart: setData</span></span>

> <span data-ttu-id="01e48-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01e48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01e48-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01e48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01e48-106">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="01e48-106">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="01e48-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01e48-107">Permissions</span></span>
<span data-ttu-id="01e48-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01e48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e48-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01e48-110">Permission type</span></span>      | <span data-ttu-id="01e48-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01e48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01e48-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01e48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01e48-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e48-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01e48-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01e48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01e48-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e48-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01e48-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01e48-116">Application</span></span> | <span data-ttu-id="01e48-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01e48-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01e48-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01e48-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="01e48-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01e48-119">Request headers</span></span>
| <span data-ttu-id="01e48-120">Nome</span><span class="sxs-lookup"><span data-stu-id="01e48-120">Name</span></span>       | <span data-ttu-id="01e48-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="01e48-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01e48-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="01e48-122">Authorization</span></span>  | <span data-ttu-id="01e48-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01e48-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01e48-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01e48-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="01e48-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="01e48-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01e48-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01e48-128">Request body</span></span>
<span data-ttu-id="01e48-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01e48-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01e48-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01e48-130">Parameter</span></span>    | <span data-ttu-id="01e48-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01e48-131">Type</span></span>   |<span data-ttu-id="01e48-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01e48-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01e48-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="01e48-133">sourceData</span></span>|<span data-ttu-id="01e48-134">string</span><span class="sxs-lookup"><span data-stu-id="01e48-134">string</span></span>|<span data-ttu-id="01e48-135">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="01e48-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="01e48-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="01e48-136">seriesBy</span></span>|<span data-ttu-id="01e48-137">string</span><span class="sxs-lookup"><span data-stu-id="01e48-137">string</span></span>|<span data-ttu-id="01e48-p105">Opcional. Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico. Pode ser um dos seguintes: automático (padrão), linhas ou colunas.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="01e48-p105">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="01e48-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="01e48-142">Response</span></span>

<span data-ttu-id="01e48-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01e48-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e48-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01e48-145">Example</span></span>
<span data-ttu-id="01e48-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="01e48-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01e48-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01e48-147">Request</span></span>
<span data-ttu-id="01e48-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01e48-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="01e48-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="01e48-149">Response</span></span>
<span data-ttu-id="01e48-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01e48-150">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
