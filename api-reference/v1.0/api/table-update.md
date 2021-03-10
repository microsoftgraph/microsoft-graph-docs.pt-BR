---
title: Atualizar tabela
description: Atualize as propriedades do objeto de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2ad466de2ded72969ddfc2645ef17101d3947f78
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577153"
---
# <a name="update-table"></a><span data-ttu-id="79f52-103">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="79f52-103">Update table</span></span>

<span data-ttu-id="79f52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f52-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79f52-105">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="79f52-105">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79f52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79f52-106">Permissions</span></span>
<span data-ttu-id="79f52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79f52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79f52-109">Permission type</span></span>      | <span data-ttu-id="79f52-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79f52-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79f52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79f52-111">Delegated (work or school account)</span></span> | <span data-ttu-id="79f52-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79f52-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79f52-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79f52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f52-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79f52-114">Not supported.</span></span>    |
|<span data-ttu-id="79f52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79f52-115">Application</span></span> | <span data-ttu-id="79f52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79f52-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79f52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79f52-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="79f52-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="79f52-118">Optional request headers</span></span>
| <span data-ttu-id="79f52-119">Nome</span><span class="sxs-lookup"><span data-stu-id="79f52-119">Name</span></span>       | <span data-ttu-id="79f52-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f52-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="79f52-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79f52-121">Authorization</span></span>  | <span data-ttu-id="79f52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79f52-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79f52-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="79f52-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="79f52-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="79f52-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79f52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79f52-127">Request body</span></span>
<span data-ttu-id="79f52-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="79f52-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79f52-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79f52-131">Property</span></span>     | <span data-ttu-id="79f52-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="79f52-132">Type</span></span>   |<span data-ttu-id="79f52-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f52-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79f52-134">nome</span><span class="sxs-lookup"><span data-stu-id="79f52-134">name</span></span>|<span data-ttu-id="79f52-135">string</span><span class="sxs-lookup"><span data-stu-id="79f52-135">string</span></span>|<span data-ttu-id="79f52-136">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="79f52-136">Name of the table.</span></span>|
|<span data-ttu-id="79f52-137">showHeaders</span><span class="sxs-lookup"><span data-stu-id="79f52-137">showHeaders</span></span>|<span data-ttu-id="79f52-138">booliano</span><span class="sxs-lookup"><span data-stu-id="79f52-138">boolean</span></span>|<span data-ttu-id="79f52-p105">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="79f52-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="79f52-141">showTotals</span><span class="sxs-lookup"><span data-stu-id="79f52-141">showTotals</span></span>|<span data-ttu-id="79f52-142">booliano</span><span class="sxs-lookup"><span data-stu-id="79f52-142">boolean</span></span>|<span data-ttu-id="79f52-p106">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="79f52-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="79f52-145">style</span><span class="sxs-lookup"><span data-stu-id="79f52-145">style</span></span>|<span data-ttu-id="79f52-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79f52-146">string</span></span>|<span data-ttu-id="79f52-147">Valor da constante que representa o estilo de Tabela.</span><span class="sxs-lookup"><span data-stu-id="79f52-147">Constant value that represents the Table style.</span></span> <span data-ttu-id="79f52-148">Os valores possíveis são: `TableStyleLight1` through , through , through `TableStyleLight21` `TableStyleMedium1`  `TableStyleMedium28` `TableStyleDark1` `TableStyleDark11` .</span><span class="sxs-lookup"><span data-stu-id="79f52-148">The possible values are: `TableStyleLight1` through `TableStyleLight21`, `TableStyleMedium1` through  `TableStyleMedium28`, `TableStyleDark1` through `TableStyleDark11`.</span></span> <span data-ttu-id="79f52-149">Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.</span><span class="sxs-lookup"><span data-stu-id="79f52-149">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="79f52-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f52-150">Response</span></span>

<span data-ttu-id="79f52-151">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [WorkbookTable](../resources/table.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79f52-151">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79f52-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79f52-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79f52-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79f52-153">Request</span></span>
<span data-ttu-id="79f52-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79f52-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79f52-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="79f52-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
# <a name="c"></a>[<span data-ttu-id="79f52-156">C#</span><span class="sxs-lookup"><span data-stu-id="79f52-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79f52-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79f52-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79f52-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79f52-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79f52-159">Java</span><span class="sxs-lookup"><span data-stu-id="79f52-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79f52-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f52-160">Response</span></span>
<span data-ttu-id="79f52-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79f52-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

