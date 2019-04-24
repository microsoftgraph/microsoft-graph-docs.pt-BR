---
title: Atualizar charttitle
description: Atualiza as propriedades do objeto charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e67790672f2e31baaacd0eba500684f7b2275e97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455805"
---
# <a name="update-charttitle"></a><span data-ttu-id="ae936-103">Atualizar charttitle</span><span class="sxs-lookup"><span data-stu-id="ae936-103">Update charttitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae936-104">Atualiza as propriedades do objeto charttitle.</span><span class="sxs-lookup"><span data-stu-id="ae936-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae936-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae936-105">Permissions</span></span>
<span data-ttu-id="ae936-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae936-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae936-108">Permission type</span></span>      | <span data-ttu-id="ae936-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae936-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae936-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae936-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae936-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae936-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae936-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae936-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae936-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae936-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae936-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae936-114">Application</span></span> | <span data-ttu-id="ae936-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae936-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae936-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae936-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="ae936-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ae936-117">Optional request headers</span></span>
| <span data-ttu-id="ae936-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ae936-118">Name</span></span>       | <span data-ttu-id="ae936-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae936-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ae936-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae936-120">Authorization</span></span>  | <span data-ttu-id="ae936-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae936-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae936-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae936-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae936-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ae936-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae936-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae936-126">Request body</span></span>
<span data-ttu-id="ae936-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ae936-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ae936-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae936-130">Property</span></span>     | <span data-ttu-id="ae936-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae936-131">Type</span></span>   |<span data-ttu-id="ae936-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae936-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae936-133">overlay</span><span class="sxs-lookup"><span data-stu-id="ae936-133">overlay</span></span>|<span data-ttu-id="ae936-134">booliano</span><span class="sxs-lookup"><span data-stu-id="ae936-134">boolean</span></span>|<span data-ttu-id="ae936-135">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="ae936-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="ae936-136">texto</span><span class="sxs-lookup"><span data-stu-id="ae936-136">text</span></span>|<span data-ttu-id="ae936-137">string</span><span class="sxs-lookup"><span data-stu-id="ae936-137">string</span></span>|<span data-ttu-id="ae936-138">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="ae936-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="ae936-139">visible</span><span class="sxs-lookup"><span data-stu-id="ae936-139">visible</span></span>|<span data-ttu-id="ae936-140">booliano</span><span class="sxs-lookup"><span data-stu-id="ae936-140">boolean</span></span>|<span data-ttu-id="ae936-141">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="ae936-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="ae936-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae936-142">Response</span></span>

<span data-ttu-id="ae936-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartTitle](../resources/charttitle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae936-143">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae936-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae936-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae936-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae936-145">Request</span></span>
<span data-ttu-id="ae936-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae936-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="ae936-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae936-147">Response</span></span>
<span data-ttu-id="ae936-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae936-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/charttitle-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
