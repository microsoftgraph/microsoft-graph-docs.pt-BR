---
title: 'Chart: setData'
description: Redefine os dados de origem do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3b8c6b31b9fd55463a67a40a0cc3e38f002d07bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456497"
---
# <a name="chart-setdata"></a><span data-ttu-id="0e735-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="0e735-103">Chart: setData</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e735-104">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="0e735-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e735-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e735-105">Permissions</span></span>
<span data-ttu-id="0e735-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e735-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e735-108">Permission type</span></span>      | <span data-ttu-id="0e735-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e735-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e735-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e735-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e735-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e735-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e735-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e735-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e735-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e735-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e735-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e735-114">Application</span></span> | <span data-ttu-id="0e735-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e735-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e735-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e735-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="0e735-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e735-117">Request headers</span></span>
| <span data-ttu-id="0e735-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0e735-118">Name</span></span>       | <span data-ttu-id="0e735-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e735-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e735-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e735-120">Authorization</span></span>  | <span data-ttu-id="0e735-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e735-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e735-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e735-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e735-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0e735-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e735-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e735-126">Request body</span></span>
<span data-ttu-id="0e735-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e735-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e735-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0e735-128">Parameter</span></span>    | <span data-ttu-id="0e735-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e735-129">Type</span></span>   |<span data-ttu-id="0e735-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e735-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e735-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="0e735-131">sourceData</span></span>|<span data-ttu-id="0e735-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e735-132">string</span></span>|<span data-ttu-id="0e735-133">O objeto Range que corresponde aos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="0e735-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="0e735-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="0e735-134">seriesBy</span></span>|<span data-ttu-id="0e735-135">string</span><span class="sxs-lookup"><span data-stu-id="0e735-135">string</span></span>|<span data-ttu-id="0e735-p104">Opcional. Especifica a forma como as colunas ou linhas são usadas como série de dados no gráfico. Pode ser um dos seguintes: automático (padrão), linhas ou colunas.  Os valores possíveis são: `Auto`, `Columns` e `Rows`.</span><span class="sxs-lookup"><span data-stu-id="0e735-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="0e735-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e735-140">Response</span></span>

<span data-ttu-id="0e735-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e735-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e735-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e735-143">Example</span></span>
<span data-ttu-id="0e735-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0e735-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e735-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e735-145">Request</span></span>
<span data-ttu-id="0e735-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e735-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0e735-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e735-147">Response</span></span>
<span data-ttu-id="0e735-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e735-148">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
