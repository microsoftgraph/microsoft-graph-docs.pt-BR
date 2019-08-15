---
title: Atualizar tabela
description: Atualize as propriedades do objeto de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1d1d7339563aa9e051907bcdf0ff49131243b69e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421446"
---
# <a name="update-table"></a><span data-ttu-id="60a3c-103">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="60a3c-103">Update table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a3c-104">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="60a3c-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60a3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="60a3c-105">Permissions</span></span>
<span data-ttu-id="60a3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60a3c-108">Permission type</span></span>      | <span data-ttu-id="60a3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60a3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60a3c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60a3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60a3c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60a3c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60a3c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60a3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a3c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60a3c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60a3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60a3c-114">Application</span></span> | <span data-ttu-id="60a3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60a3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60a3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="60a3c-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="60a3c-117">Optional request headers</span></span>
| <span data-ttu-id="60a3c-118">Name</span><span class="sxs-lookup"><span data-stu-id="60a3c-118">Name</span></span>       | <span data-ttu-id="60a3c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a3c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="60a3c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="60a3c-120">Authorization</span></span>  | <span data-ttu-id="60a3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60a3c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60a3c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="60a3c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a3c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60a3c-126">Request body</span></span>
<span data-ttu-id="60a3c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60a3c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60a3c-130">Property</span></span>     | <span data-ttu-id="60a3c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60a3c-131">Type</span></span>   |<span data-ttu-id="60a3c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a3c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60a3c-133">name</span><span class="sxs-lookup"><span data-stu-id="60a3c-133">name</span></span>|<span data-ttu-id="60a3c-134">string</span><span class="sxs-lookup"><span data-stu-id="60a3c-134">string</span></span>|<span data-ttu-id="60a3c-135">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="60a3c-135">Name of the table.</span></span>|
|<span data-ttu-id="60a3c-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="60a3c-136">showHeaders</span></span>|<span data-ttu-id="60a3c-137">booliano</span><span class="sxs-lookup"><span data-stu-id="60a3c-137">boolean</span></span>|<span data-ttu-id="60a3c-p105">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="60a3c-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="60a3c-140">showTotals</span></span>|<span data-ttu-id="60a3c-141">booliano</span><span class="sxs-lookup"><span data-stu-id="60a3c-141">boolean</span></span>|<span data-ttu-id="60a3c-p106">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="60a3c-144">style</span><span class="sxs-lookup"><span data-stu-id="60a3c-144">style</span></span>|<span data-ttu-id="60a3c-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60a3c-145">string</span></span>|<span data-ttu-id="60a3c-p107">Valor da constante que representa o estilo de Tabela. Os valores possíveis são: TableStyleLight1 a TableStyleLight21, TableStyleMedium1 a TableStyleMedium28, TableStyleStyleDark1 a TableStyleStyleDark11. Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p107">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="60a3c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a3c-149">Response</span></span>

<span data-ttu-id="60a3c-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Table](../resources/workbooktable.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60a3c-150">If successful, this method returns a `200 OK` response code and updated [Table](../resources/workbooktable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60a3c-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60a3c-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60a3c-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60a3c-152">Request</span></span>
<span data-ttu-id="60a3c-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60a3c-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60a3c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="60a3c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a3c-155">C#</span><span class="sxs-lookup"><span data-stu-id="60a3c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a3c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a3c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a3c-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="60a3c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60a3c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a3c-158">Response</span></span>
<span data-ttu-id="60a3c-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60a3c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
