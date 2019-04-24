---
title: Atualizar chartfont
description: Atualiza as propriedades do objeto chartfont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4878e78690cc0b28f686d4f0c3c678325397cc07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456505"
---
# <a name="update-chartfont"></a><span data-ttu-id="b0ad0-103">Atualizar chartfont</span><span class="sxs-lookup"><span data-stu-id="b0ad0-103">Update chartfont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ad0-104">Atualiza as propriedades do objeto chartfont.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-104">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0ad0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0ad0-105">Permissions</span></span>
<span data-ttu-id="b0ad0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0ad0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0ad0-108">Permission type</span></span>      | <span data-ttu-id="b0ad0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0ad0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ad0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0ad0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ad0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ad0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0ad0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0ad0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ad0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ad0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0ad0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0ad0-114">Application</span></span> | <span data-ttu-id="b0ad0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ad0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0ad0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="b0ad0-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b0ad0-117">Optional request headers</span></span>
| <span data-ttu-id="b0ad0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b0ad0-118">Name</span></span>       | <span data-ttu-id="b0ad0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ad0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b0ad0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0ad0-120">Authorization</span></span>  | <span data-ttu-id="b0ad0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0ad0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b0ad0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b0ad0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0ad0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0ad0-126">Request body</span></span>
<span data-ttu-id="b0ad0-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b0ad0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0ad0-130">Property</span></span>     | <span data-ttu-id="b0ad0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0ad0-131">Type</span></span>   |<span data-ttu-id="b0ad0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ad0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0ad0-133">bold</span><span class="sxs-lookup"><span data-stu-id="b0ad0-133">bold</span></span>|<span data-ttu-id="b0ad0-134">booliano</span><span class="sxs-lookup"><span data-stu-id="b0ad0-134">boolean</span></span>|<span data-ttu-id="b0ad0-135">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="b0ad0-136">color</span><span class="sxs-lookup"><span data-stu-id="b0ad0-136">color</span></span>|<span data-ttu-id="b0ad0-137">string</span><span class="sxs-lookup"><span data-stu-id="b0ad0-137">string</span></span>|<span data-ttu-id="b0ad0-p105">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="b0ad0-141">italic</span><span class="sxs-lookup"><span data-stu-id="b0ad0-141">italic</span></span>|<span data-ttu-id="b0ad0-142">booliano</span><span class="sxs-lookup"><span data-stu-id="b0ad0-142">boolean</span></span>|<span data-ttu-id="b0ad0-143">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="b0ad0-144">nome</span><span class="sxs-lookup"><span data-stu-id="b0ad0-144">name</span></span>|<span data-ttu-id="b0ad0-145">string</span><span class="sxs-lookup"><span data-stu-id="b0ad0-145">string</span></span>|<span data-ttu-id="b0ad0-146">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="b0ad0-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="b0ad0-147">size</span><span class="sxs-lookup"><span data-stu-id="b0ad0-147">size</span></span>|<span data-ttu-id="b0ad0-148">Double</span><span class="sxs-lookup"><span data-stu-id="b0ad0-148">double</span></span>|<span data-ttu-id="b0ad0-149">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-149">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="b0ad0-150">underline</span><span class="sxs-lookup"><span data-stu-id="b0ad0-150">underline</span></span>|<span data-ttu-id="b0ad0-151">string</span><span class="sxs-lookup"><span data-stu-id="b0ad0-151">string</span></span>|<span data-ttu-id="b0ad0-p106">Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` e `Single`.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="b0ad0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0ad0-154">Response</span></span>

<span data-ttu-id="b0ad0-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartFont](../resources/chartfont.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-155">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0ad0-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0ad0-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0ad0-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0ad0-157">Request</span></span>
<span data-ttu-id="b0ad0-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b0ad0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0ad0-159">Response</span></span>
<span data-ttu-id="b0ad0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0ad0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfont-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
