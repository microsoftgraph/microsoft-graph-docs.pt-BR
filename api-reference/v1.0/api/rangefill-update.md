---
title: Atualizar rangefill
description: Atualize as propriedades do objeto rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 08dcc5f9181354f394741fffa036375a865b53b7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034963"
---
# <a name="update-rangefill"></a><span data-ttu-id="8b9ab-103">Atualizar rangefill</span><span class="sxs-lookup"><span data-stu-id="8b9ab-103">Update rangefill</span></span>

<span data-ttu-id="8b9ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b9ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b9ab-105">Atualize as propriedades do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-105">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b9ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b9ab-106">Permissions</span></span>
<span data-ttu-id="8b9ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b9ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b9ab-109">Permission type</span></span>      | <span data-ttu-id="8b9ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b9ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b9ab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b9ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b9ab-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b9ab-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b9ab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b9ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b9ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-114">Not supported.</span></span>    |
|<span data-ttu-id="8b9ab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b9ab-115">Application</span></span> | <span data-ttu-id="8b9ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b9ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b9ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/fill
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="8b9ab-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8b9ab-118">Optional request headers</span></span>
| <span data-ttu-id="8b9ab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8b9ab-119">Name</span></span>       | <span data-ttu-id="8b9ab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b9ab-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8b9ab-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b9ab-121">Authorization</span></span>  | <span data-ttu-id="8b9ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b9ab-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8b9ab-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b9ab-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b9ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9ab-127">Request body</span></span>
<span data-ttu-id="8b9ab-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8b9ab-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b9ab-131">Property</span></span>     | <span data-ttu-id="8b9ab-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b9ab-132">Type</span></span>   |<span data-ttu-id="8b9ab-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b9ab-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b9ab-134">color</span><span class="sxs-lookup"><span data-stu-id="8b9ab-134">color</span></span>|<span data-ttu-id="8b9ab-135">string</span><span class="sxs-lookup"><span data-stu-id="8b9ab-135">string</span></span>|<span data-ttu-id="8b9ab-136">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="8b9ab-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="8b9ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b9ab-137">Response</span></span>

<span data-ttu-id="8b9ab-138">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookRangeFill](../resources/rangefill.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-138">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b9ab-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b9ab-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b9ab-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9ab-140">Request</span></span>
<span data-ttu-id="8b9ab-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b9ab-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b9ab-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b9ab-143">C#</span><span class="sxs-lookup"><span data-stu-id="8b9ab-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b9ab-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b9ab-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b9ab-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b9ab-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b9ab-146">Java</span><span class="sxs-lookup"><span data-stu-id="8b9ab-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b9ab-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b9ab-147">Response</span></span>
<span data-ttu-id="8b9ab-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-148">Here is an example of the response.</span></span> <span data-ttu-id="8b9ab-149">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b9ab-149">Note: The response object shown here might be shortened for readability.</span></span>
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

