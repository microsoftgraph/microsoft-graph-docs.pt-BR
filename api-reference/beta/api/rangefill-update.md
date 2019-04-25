---
title: Atualizar rangefill
description: Atualize as propriedades do objeto rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 87214cf944c5f0aadd26189dcdfba6383cb6cb65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546226"
---
# <a name="update-rangefill"></a><span data-ttu-id="d0610-103">Atualizar rangefill</span><span class="sxs-lookup"><span data-stu-id="d0610-103">Update rangefill</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0610-104">Atualize as propriedades do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="d0610-104">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0610-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0610-105">Permissions</span></span>
<span data-ttu-id="d0610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0610-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0610-108">Permission type</span></span>      | <span data-ttu-id="d0610-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0610-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0610-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0610-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0610-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0610-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d0610-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0610-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0610-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0610-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d0610-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0610-114">Application</span></span> | <span data-ttu-id="d0610-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0610-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0610-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0610-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="d0610-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d0610-117">Optional request headers</span></span>
| <span data-ttu-id="d0610-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d0610-118">Name</span></span>       | <span data-ttu-id="d0610-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0610-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0610-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0610-120">Authorization</span></span>  | <span data-ttu-id="d0610-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0610-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0610-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d0610-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d0610-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d0610-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0610-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0610-126">Request body</span></span>
<span data-ttu-id="d0610-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d0610-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0610-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0610-130">Property</span></span>     | <span data-ttu-id="d0610-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0610-131">Type</span></span>   |<span data-ttu-id="d0610-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0610-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0610-133">color</span><span class="sxs-lookup"><span data-stu-id="d0610-133">color</span></span>|<span data-ttu-id="d0610-134">string</span><span class="sxs-lookup"><span data-stu-id="d0610-134">string</span></span>|<span data-ttu-id="d0610-135">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="d0610-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="d0610-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0610-136">Response</span></span>

<span data-ttu-id="d0610-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFill](../resources/rangefill.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0610-137">If successful, this method returns a `200 OK` response code and updated [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0610-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0610-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0610-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0610-139">Request</span></span>
<span data-ttu-id="d0610-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0610-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="d0610-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0610-141">Response</span></span>
<span data-ttu-id="d0610-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0610-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangefill-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
