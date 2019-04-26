---
title: Atualizar chartlineformat
description: Atualiza as propriedades do objeto chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 860b0aaf39211131a2ea346d9cbe95749631e17a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327758"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="7c1cd-103">Atualizar chartlineformat</span><span class="sxs-lookup"><span data-stu-id="7c1cd-103">Update chartlineformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c1cd-104">Atualiza as propriedades do objeto chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-104">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c1cd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c1cd-105">Permissions</span></span>
<span data-ttu-id="7c1cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c1cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c1cd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c1cd-108">Permission type</span></span>      | <span data-ttu-id="7c1cd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c1cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c1cd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c1cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c1cd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c1cd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c1cd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c1cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c1cd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c1cd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c1cd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c1cd-114">Application</span></span> | <span data-ttu-id="7c1cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c1cd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c1cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="7c1cd-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7c1cd-117">Optional request headers</span></span>
| <span data-ttu-id="7c1cd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7c1cd-118">Name</span></span>       | <span data-ttu-id="7c1cd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c1cd-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7c1cd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c1cd-120">Authorization</span></span>  | <span data-ttu-id="7c1cd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c1cd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c1cd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c1cd-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c1cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c1cd-126">Request body</span></span>
<span data-ttu-id="7c1cd-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7c1cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c1cd-130">Property</span></span>     | <span data-ttu-id="7c1cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c1cd-131">Type</span></span>   |<span data-ttu-id="7c1cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c1cd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c1cd-133">color</span><span class="sxs-lookup"><span data-stu-id="7c1cd-133">color</span></span>|<span data-ttu-id="7c1cd-134">string</span><span class="sxs-lookup"><span data-stu-id="7c1cd-134">string</span></span>|<span data-ttu-id="7c1cd-135">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-135">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="7c1cd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c1cd-136">Response</span></span>

<span data-ttu-id="7c1cd-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartLineFormat](../resources/workbookchartlineformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-137">If successful, this method returns a `200 OK` response code and updated [workbookChartLineFormat](../resources/workbookchartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c1cd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c1cd-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c1cd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c1cd-139">Request</span></span>
<span data-ttu-id="7c1cd-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="7c1cd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c1cd-141">Response</span></span>
<span data-ttu-id="7c1cd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c1cd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
