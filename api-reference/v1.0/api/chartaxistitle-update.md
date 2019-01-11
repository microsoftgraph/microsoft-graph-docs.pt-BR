---
title: Atualizar chartaxistitle
description: Atualiza as propriedades do objeto chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 692cf189c3eb4824c5b4dd9b56048434f4b3cfa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836670"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="746fc-103">Atualizar chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="746fc-103">Update chartaxistitle</span></span>

<span data-ttu-id="746fc-104">Atualiza as propriedades do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="746fc-104">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="746fc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="746fc-105">Permissions</span></span>
<span data-ttu-id="746fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="746fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="746fc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="746fc-108">Permission type</span></span>      | <span data-ttu-id="746fc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="746fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="746fc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="746fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="746fc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="746fc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="746fc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="746fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="746fc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="746fc-113">Not supported.</span></span>    |
|<span data-ttu-id="746fc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="746fc-114">Application</span></span> | <span data-ttu-id="746fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="746fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="746fc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="746fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="746fc-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="746fc-117">Optional request headers</span></span>
| <span data-ttu-id="746fc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="746fc-118">Name</span></span>       | <span data-ttu-id="746fc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="746fc-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="746fc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="746fc-120">Authorization</span></span>  | <span data-ttu-id="746fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="746fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="746fc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="746fc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="746fc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="746fc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="746fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="746fc-126">Request body</span></span>
<span data-ttu-id="746fc-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="746fc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="746fc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="746fc-130">Property</span></span>     | <span data-ttu-id="746fc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="746fc-131">Type</span></span>   |<span data-ttu-id="746fc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="746fc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="746fc-133">texto</span><span class="sxs-lookup"><span data-stu-id="746fc-133">text</span></span>|<span data-ttu-id="746fc-134">string</span><span class="sxs-lookup"><span data-stu-id="746fc-134">string</span></span>|<span data-ttu-id="746fc-135">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="746fc-135">Represents the axis title.</span></span>|
|<span data-ttu-id="746fc-136">visible</span><span class="sxs-lookup"><span data-stu-id="746fc-136">visible</span></span>|<span data-ttu-id="746fc-137">booliano</span><span class="sxs-lookup"><span data-stu-id="746fc-137">boolean</span></span>|<span data-ttu-id="746fc-138">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="746fc-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="746fc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="746fc-139">Response</span></span>

<span data-ttu-id="746fc-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookChartAxisTitle](../resources/chartaxistitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="746fc-140">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="746fc-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="746fc-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="746fc-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746fc-142">Request</span></span>
<span data-ttu-id="746fc-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="746fc-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="746fc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="746fc-144">Response</span></span>
<span data-ttu-id="746fc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="746fc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
