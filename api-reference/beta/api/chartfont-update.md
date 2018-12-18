---
title: Atualizar chartfont
description: Atualiza as propriedades do objeto chartfont.
author: lumine2008
ms.openlocfilehash: 335a7eb278ce1d5cd6ffee5a96222ec5a189aefa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328200"
---
# <a name="update-chartfont"></a><span data-ttu-id="d3a25-103">Atualizar chartfont</span><span class="sxs-lookup"><span data-stu-id="d3a25-103">Update chartfont</span></span>

> <span data-ttu-id="d3a25-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3a25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3a25-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3a25-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3a25-106">Atualiza as propriedades do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="d3a25-106">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3a25-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3a25-107">Permissions</span></span>
<span data-ttu-id="d3a25-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a25-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3a25-110">Permission type</span></span>      | <span data-ttu-id="d3a25-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3a25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3a25-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3a25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3a25-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3a25-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3a25-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3a25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3a25-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3a25-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3a25-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3a25-116">Application</span></span> | <span data-ttu-id="d3a25-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a25-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3a25-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a25-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="d3a25-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d3a25-119">Optional request headers</span></span>
| <span data-ttu-id="d3a25-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d3a25-120">Name</span></span>       | <span data-ttu-id="d3a25-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3a25-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d3a25-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3a25-122">Authorization</span></span>  | <span data-ttu-id="d3a25-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3a25-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3a25-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3a25-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3a25-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3a25-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a25-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a25-128">Request body</span></span>
<span data-ttu-id="d3a25-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d3a25-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d3a25-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3a25-132">Property</span></span>     | <span data-ttu-id="d3a25-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3a25-133">Type</span></span>   |<span data-ttu-id="d3a25-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3a25-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3a25-135">bold</span><span class="sxs-lookup"><span data-stu-id="d3a25-135">bold</span></span>|<span data-ttu-id="d3a25-136">booliano</span><span class="sxs-lookup"><span data-stu-id="d3a25-136">boolean</span></span>|<span data-ttu-id="d3a25-137">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="d3a25-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="d3a25-138">color</span><span class="sxs-lookup"><span data-stu-id="d3a25-138">color</span></span>|<span data-ttu-id="d3a25-139">string</span><span class="sxs-lookup"><span data-stu-id="d3a25-139">string</span></span>|<span data-ttu-id="d3a25-p106">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="d3a25-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="d3a25-143">italic</span><span class="sxs-lookup"><span data-stu-id="d3a25-143">italic</span></span>|<span data-ttu-id="d3a25-144">booliano</span><span class="sxs-lookup"><span data-stu-id="d3a25-144">boolean</span></span>|<span data-ttu-id="d3a25-145">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="d3a25-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="d3a25-146">name</span><span class="sxs-lookup"><span data-stu-id="d3a25-146">name</span></span>|<span data-ttu-id="d3a25-147">string</span><span class="sxs-lookup"><span data-stu-id="d3a25-147">string</span></span>|<span data-ttu-id="d3a25-148">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="d3a25-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="d3a25-149">size</span><span class="sxs-lookup"><span data-stu-id="d3a25-149">size</span></span>|<span data-ttu-id="d3a25-150">Double</span><span class="sxs-lookup"><span data-stu-id="d3a25-150">double</span></span>|<span data-ttu-id="d3a25-151">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="d3a25-151">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="d3a25-152">underline</span><span class="sxs-lookup"><span data-stu-id="d3a25-152">underline</span></span>|<span data-ttu-id="d3a25-153">string</span><span class="sxs-lookup"><span data-stu-id="d3a25-153">string</span></span>|<span data-ttu-id="d3a25-p107">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="d3a25-p107">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="d3a25-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a25-156">Response</span></span>

<span data-ttu-id="d3a25-157">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartFont](../resources/chartfont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a25-157">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3a25-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3a25-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3a25-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a25-159">Request</span></span>
<span data-ttu-id="d3a25-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3a25-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
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
##### <a name="response"></a><span data-ttu-id="d3a25-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a25-161">Response</span></span>
<span data-ttu-id="d3a25-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3a25-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->