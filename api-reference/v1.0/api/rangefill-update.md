---
title: Atualizar rangefill
description: Atualize as propriedades do objeto rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0327ace462d3e9f10697392f03203cbddd36b8cc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459766"
---
# <a name="update-rangefill"></a><span data-ttu-id="eea3a-103">Atualizar rangefill</span><span class="sxs-lookup"><span data-stu-id="eea3a-103">Update rangefill</span></span>

<span data-ttu-id="eea3a-104">Atualize as propriedades do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="eea3a-104">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eea3a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eea3a-105">Permissions</span></span>
<span data-ttu-id="eea3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eea3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea3a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eea3a-108">Permission type</span></span>      | <span data-ttu-id="eea3a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eea3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eea3a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eea3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eea3a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea3a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eea3a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eea3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eea3a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eea3a-113">Not supported.</span></span>    |
|<span data-ttu-id="eea3a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eea3a-114">Application</span></span> | <span data-ttu-id="eea3a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eea3a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eea3a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eea3a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="eea3a-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="eea3a-117">Optional request headers</span></span>
| <span data-ttu-id="eea3a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eea3a-118">Name</span></span>       | <span data-ttu-id="eea3a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="eea3a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eea3a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="eea3a-120">Authorization</span></span>  | <span data-ttu-id="eea3a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eea3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eea3a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eea3a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="eea3a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eea3a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea3a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eea3a-126">Request body</span></span>
<span data-ttu-id="eea3a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eea3a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eea3a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eea3a-130">Property</span></span>     | <span data-ttu-id="eea3a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eea3a-131">Type</span></span>   |<span data-ttu-id="eea3a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eea3a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eea3a-133">color</span><span class="sxs-lookup"><span data-stu-id="eea3a-133">color</span></span>|<span data-ttu-id="eea3a-134">string</span><span class="sxs-lookup"><span data-stu-id="eea3a-134">string</span></span>|<span data-ttu-id="eea3a-135">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="eea3a-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="eea3a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eea3a-136">Response</span></span>

<span data-ttu-id="eea3a-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookRangeFill](../resources/rangefill.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eea3a-137">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eea3a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eea3a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eea3a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eea3a-139">Request</span></span>
<span data-ttu-id="eea3a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eea3a-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eea3a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="eea3a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eea3a-142">C#</span><span class="sxs-lookup"><span data-stu-id="eea3a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eea3a-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="eea3a-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eea3a-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eea3a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eea3a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="eea3a-145">Response</span></span>
<span data-ttu-id="eea3a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eea3a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
