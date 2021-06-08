---
title: Atualizar rangefill
description: Atualize as propriedades do objeto rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2f88d753e8d8e5a541c42feca9bd60084a41412e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785883"
---
# <a name="update-rangefill"></a><span data-ttu-id="a3871-103">Atualizar rangefill</span><span class="sxs-lookup"><span data-stu-id="a3871-103">Update rangefill</span></span>

<span data-ttu-id="a3871-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3871-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3871-105">Atualize as propriedades do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="a3871-105">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3871-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a3871-106">Permissions</span></span>
<span data-ttu-id="a3871-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3871-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3871-109">Permission type</span></span>      | <span data-ttu-id="a3871-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3871-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3871-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3871-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3871-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3871-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a3871-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3871-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3871-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3871-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a3871-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3871-115">Application</span></span> | <span data-ttu-id="a3871-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3871-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3871-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3871-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/fill
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="a3871-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a3871-118">Optional request headers</span></span>
| <span data-ttu-id="a3871-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a3871-119">Name</span></span>       | <span data-ttu-id="a3871-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3871-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a3871-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3871-121">Authorization</span></span>  | <span data-ttu-id="a3871-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3871-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3871-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a3871-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a3871-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a3871-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3871-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3871-127">Request body</span></span>
<span data-ttu-id="a3871-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a3871-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a3871-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3871-131">Property</span></span>     | <span data-ttu-id="a3871-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3871-132">Type</span></span>   |<span data-ttu-id="a3871-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3871-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3871-134">color</span><span class="sxs-lookup"><span data-stu-id="a3871-134">color</span></span>|<span data-ttu-id="a3871-135">string</span><span class="sxs-lookup"><span data-stu-id="a3871-135">string</span></span>|<span data-ttu-id="a3871-136">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="a3871-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="a3871-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3871-137">Response</span></span>

<span data-ttu-id="a3871-138">Se tiver êxito, este método retornará um código de resposta e `200 OK` um objeto [workbookRangeFill](../resources/workbookrangefill.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3871-138">If successful, this method returns a `200 OK` response code and updated [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3871-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3871-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3871-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3871-140">Request</span></span>
<span data-ttu-id="a3871-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3871-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3871-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3871-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="a3871-143">C#</span><span class="sxs-lookup"><span data-stu-id="a3871-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3871-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3871-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3871-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3871-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3871-146">Java</span><span class="sxs-lookup"><span data-stu-id="a3871-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangefill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a3871-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3871-147">Response</span></span>
<span data-ttu-id="a3871-p105">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="a3871-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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
  ]
}
-->


