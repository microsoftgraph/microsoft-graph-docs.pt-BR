---
title: Atualizar rangefont
description: Atualize as propriedades do objeto rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 40dfe68ec16415dbfa4abcbdb46da8cc9f89c961
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927300"
---
# <a name="update-rangefont"></a><span data-ttu-id="76201-103">Atualizar rangefont</span><span class="sxs-lookup"><span data-stu-id="76201-103">Update rangefont</span></span>

<span data-ttu-id="76201-104">Atualize as propriedades do objeto rangefont.</span><span class="sxs-lookup"><span data-stu-id="76201-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="76201-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="76201-105">Permissions</span></span>
<span data-ttu-id="76201-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76201-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76201-108">Permission type</span></span>      | <span data-ttu-id="76201-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76201-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76201-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76201-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76201-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76201-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="76201-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76201-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76201-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76201-113">Not supported.</span></span>    |
|<span data-ttu-id="76201-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76201-114">Application</span></span> | <span data-ttu-id="76201-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76201-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76201-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76201-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="request-headers"></a><span data-ttu-id="76201-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76201-117">Request headers</span></span>
| <span data-ttu-id="76201-118">Nome</span><span class="sxs-lookup"><span data-stu-id="76201-118">Name</span></span>       | <span data-ttu-id="76201-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="76201-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="76201-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="76201-120">Authorization</span></span>  | <span data-ttu-id="76201-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76201-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76201-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76201-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="76201-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="76201-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76201-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76201-126">Request body</span></span>
<span data-ttu-id="76201-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="76201-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76201-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76201-130">Property</span></span>     | <span data-ttu-id="76201-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76201-131">Type</span></span>   |<span data-ttu-id="76201-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76201-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76201-133">bold</span><span class="sxs-lookup"><span data-stu-id="76201-133">bold</span></span>|<span data-ttu-id="76201-134">booliano</span><span class="sxs-lookup"><span data-stu-id="76201-134">boolean</span></span>|<span data-ttu-id="76201-135">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="76201-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="76201-136">color</span><span class="sxs-lookup"><span data-stu-id="76201-136">color</span></span>|<span data-ttu-id="76201-137">string</span><span class="sxs-lookup"><span data-stu-id="76201-137">string</span></span>|<span data-ttu-id="76201-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="76201-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="76201-141">italic</span><span class="sxs-lookup"><span data-stu-id="76201-141">italic</span></span>|<span data-ttu-id="76201-142">booliano</span><span class="sxs-lookup"><span data-stu-id="76201-142">boolean</span></span>|<span data-ttu-id="76201-143">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="76201-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="76201-144">name</span><span class="sxs-lookup"><span data-stu-id="76201-144">name</span></span>|<span data-ttu-id="76201-145">string</span><span class="sxs-lookup"><span data-stu-id="76201-145">string</span></span>|<span data-ttu-id="76201-146">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="76201-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="76201-147">size</span><span class="sxs-lookup"><span data-stu-id="76201-147">size</span></span>|<span data-ttu-id="76201-148">Double</span><span class="sxs-lookup"><span data-stu-id="76201-148">double</span></span>|<span data-ttu-id="76201-149">Font Size</span><span class="sxs-lookup"><span data-stu-id="76201-149">Font size.</span></span>|
|<span data-ttu-id="76201-150">underline</span><span class="sxs-lookup"><span data-stu-id="76201-150">underline</span></span>|<span data-ttu-id="76201-151">string</span><span class="sxs-lookup"><span data-stu-id="76201-151">string</span></span>|<span data-ttu-id="76201-152">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="76201-152">Type of underline applied to the font.</span></span> <span data-ttu-id="76201-153">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="76201-153">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="76201-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="76201-154">Response</span></span>

<span data-ttu-id="76201-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookRangeFont](../resources/rangefont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76201-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76201-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76201-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76201-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76201-157">Request</span></span>
<span data-ttu-id="76201-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76201-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="76201-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="76201-159">Response</span></span>
<span data-ttu-id="76201-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76201-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
