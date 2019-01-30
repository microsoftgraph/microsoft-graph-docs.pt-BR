---
title: 'ChartSeriesCollection: ItemAt'
description: Recupera uma série com base na respectiva posição na coleção.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 063a5a605908693e5b189c92865eaec2c0dba1ba
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640249"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="7432a-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="7432a-103">ChartSeriesCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7432a-104">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="7432a-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="7432a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7432a-105">Permissions</span></span>
<span data-ttu-id="7432a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7432a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7432a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7432a-108">Permission type</span></span>      | <span data-ttu-id="7432a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7432a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7432a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7432a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7432a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7432a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7432a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7432a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7432a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7432a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7432a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7432a-114">Application</span></span> | <span data-ttu-id="7432a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7432a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7432a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7432a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="7432a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7432a-117">Request headers</span></span>
| <span data-ttu-id="7432a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7432a-118">Name</span></span>       | <span data-ttu-id="7432a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7432a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7432a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7432a-120">Authorization</span></span>  | <span data-ttu-id="7432a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7432a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7432a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7432a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7432a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7432a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7432a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7432a-126">Request body</span></span>
<span data-ttu-id="7432a-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7432a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7432a-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7432a-128">Parameter</span></span>    | <span data-ttu-id="7432a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7432a-129">Type</span></span>   |<span data-ttu-id="7432a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7432a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7432a-131">índice</span><span class="sxs-lookup"><span data-stu-id="7432a-131">index</span></span>|<span data-ttu-id="7432a-132">number</span><span class="sxs-lookup"><span data-stu-id="7432a-132">number</span></span>|<span data-ttu-id="7432a-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="7432a-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7432a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7432a-135">Response</span></span>

<span data-ttu-id="7432a-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7432a-136">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7432a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7432a-137">Example</span></span>
<span data-ttu-id="7432a-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7432a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7432a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7432a-139">Request</span></span>
<span data-ttu-id="7432a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7432a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="7432a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7432a-141">Response</span></span>
<span data-ttu-id="7432a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7432a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseriescollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
