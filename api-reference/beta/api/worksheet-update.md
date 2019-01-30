---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bf726ce3ad9bff427b3ec78d572017f6aea162e4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641537"
---
# <a name="update-worksheet"></a><span data-ttu-id="e1de5-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="e1de5-103">Update worksheet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1de5-104">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="e1de5-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1de5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1de5-105">Permissions</span></span>
<span data-ttu-id="e1de5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1de5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1de5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1de5-108">Permission type</span></span>      | <span data-ttu-id="e1de5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1de5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1de5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1de5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1de5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1de5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e1de5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1de5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1de5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1de5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e1de5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1de5-114">Application</span></span> | <span data-ttu-id="e1de5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1de5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1de5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1de5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e1de5-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e1de5-117">Optional request headers</span></span>
| <span data-ttu-id="e1de5-118">Name</span><span class="sxs-lookup"><span data-stu-id="e1de5-118">Name</span></span>       | <span data-ttu-id="e1de5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1de5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e1de5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1de5-120">Authorization</span></span>  | <span data-ttu-id="e1de5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1de5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1de5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e1de5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e1de5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1de5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1de5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1de5-126">Request body</span></span>
<span data-ttu-id="e1de5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e1de5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e1de5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1de5-130">Property</span></span>     | <span data-ttu-id="e1de5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1de5-131">Type</span></span>   |<span data-ttu-id="e1de5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1de5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1de5-133">name</span><span class="sxs-lookup"><span data-stu-id="e1de5-133">name</span></span>|<span data-ttu-id="e1de5-134">string</span><span class="sxs-lookup"><span data-stu-id="e1de5-134">string</span></span>|<span data-ttu-id="e1de5-135">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="e1de5-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="e1de5-136">position</span><span class="sxs-lookup"><span data-stu-id="e1de5-136">position</span></span>|<span data-ttu-id="e1de5-137">int</span><span class="sxs-lookup"><span data-stu-id="e1de5-137">int</span></span>|<span data-ttu-id="e1de5-138">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e1de5-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="e1de5-139">visibilidade</span><span class="sxs-lookup"><span data-stu-id="e1de5-139">visibility</span></span>|<span data-ttu-id="e1de5-140">string</span><span class="sxs-lookup"><span data-stu-id="e1de5-140">string</span></span>|<span data-ttu-id="e1de5-p105">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="e1de5-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="e1de5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1de5-143">Response</span></span>

<span data-ttu-id="e1de5-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1de5-144">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1de5-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1de5-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1de5-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1de5-146">Request</span></span>
<span data-ttu-id="e1de5-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1de5-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="e1de5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1de5-148">Response</span></span>
<span data-ttu-id="e1de5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1de5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
