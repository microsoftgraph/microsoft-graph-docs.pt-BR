---
title: Atualizar chartgridlines
description: Atualiza as propriedades do objeto chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7c50504923b807b2eb5dbbccb964d16262284b8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927662"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="357c2-103">Atualizar chartgridlines</span><span class="sxs-lookup"><span data-stu-id="357c2-103">Update chartgridlines</span></span>

<span data-ttu-id="357c2-104">Atualiza as propriedades do objeto chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="357c2-104">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="357c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="357c2-105">Permissions</span></span>
<span data-ttu-id="357c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="357c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="357c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="357c2-108">Permission type</span></span>      | <span data-ttu-id="357c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="357c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="357c2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="357c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="357c2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="357c2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="357c2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="357c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="357c2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357c2-113">Not supported.</span></span>    |
|<span data-ttu-id="357c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="357c2-114">Application</span></span> | <span data-ttu-id="357c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="357c2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="357c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="357c2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="357c2-117">Request headers</span></span>
| <span data-ttu-id="357c2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="357c2-118">Name</span></span>       | <span data-ttu-id="357c2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="357c2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="357c2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="357c2-120">Authorization</span></span>  | <span data-ttu-id="357c2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="357c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="357c2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="357c2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="357c2-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="357c2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="357c2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="357c2-126">Request body</span></span>
<span data-ttu-id="357c2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="357c2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="357c2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="357c2-130">Property</span></span>     | <span data-ttu-id="357c2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="357c2-131">Type</span></span>   |<span data-ttu-id="357c2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="357c2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="357c2-133">visible</span><span class="sxs-lookup"><span data-stu-id="357c2-133">visible</span></span>|<span data-ttu-id="357c2-134">booliano</span><span class="sxs-lookup"><span data-stu-id="357c2-134">boolean</span></span>|<span data-ttu-id="357c2-135">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="357c2-135">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="357c2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="357c2-136">Response</span></span>

<span data-ttu-id="357c2-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookChartGridlines](../resources/chartgridlines.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="357c2-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="357c2-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="357c2-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="357c2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="357c2-139">Request</span></span>
<span data-ttu-id="357c2-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="357c2-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="357c2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="357c2-141">Response</span></span>
<span data-ttu-id="357c2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="357c2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
