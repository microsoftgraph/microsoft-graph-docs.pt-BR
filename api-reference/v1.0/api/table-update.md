---
title: Atualizar tabela
description: Atualize as propriedades do objeto de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a3e544e06519dfd014eb70eec5eb0cf4d84d4996
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509616"
---
# <a name="update-table"></a><span data-ttu-id="36f0a-103">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="36f0a-103">Update table</span></span>

<span data-ttu-id="36f0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36f0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36f0a-105">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="36f0a-105">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36f0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36f0a-106">Permissions</span></span>
<span data-ttu-id="36f0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36f0a-109">Permission type</span></span>      | <span data-ttu-id="36f0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36f0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36f0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36f0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36f0a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36f0a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36f0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36f0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36f0a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36f0a-114">Not supported.</span></span>    |
|<span data-ttu-id="36f0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36f0a-115">Application</span></span> | <span data-ttu-id="36f0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36f0a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36f0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36f0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="36f0a-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="36f0a-118">Optional request headers</span></span>
| <span data-ttu-id="36f0a-119">Name</span><span class="sxs-lookup"><span data-stu-id="36f0a-119">Name</span></span>       | <span data-ttu-id="36f0a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="36f0a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36f0a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="36f0a-121">Authorization</span></span>  | <span data-ttu-id="36f0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36f0a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36f0a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36f0a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="36f0a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="36f0a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36f0a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36f0a-127">Request body</span></span>
<span data-ttu-id="36f0a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="36f0a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36f0a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36f0a-131">Property</span></span>     | <span data-ttu-id="36f0a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="36f0a-132">Type</span></span>   |<span data-ttu-id="36f0a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="36f0a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36f0a-134">nome</span><span class="sxs-lookup"><span data-stu-id="36f0a-134">name</span></span>|<span data-ttu-id="36f0a-135">string</span><span class="sxs-lookup"><span data-stu-id="36f0a-135">string</span></span>|<span data-ttu-id="36f0a-136">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="36f0a-136">Name of the table.</span></span>|
|<span data-ttu-id="36f0a-137">showHeaders</span><span class="sxs-lookup"><span data-stu-id="36f0a-137">showHeaders</span></span>|<span data-ttu-id="36f0a-138">booliano</span><span class="sxs-lookup"><span data-stu-id="36f0a-138">boolean</span></span>|<span data-ttu-id="36f0a-p105">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="36f0a-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="36f0a-141">showTotals</span><span class="sxs-lookup"><span data-stu-id="36f0a-141">showTotals</span></span>|<span data-ttu-id="36f0a-142">booliano</span><span class="sxs-lookup"><span data-stu-id="36f0a-142">boolean</span></span>|<span data-ttu-id="36f0a-p106">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="36f0a-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="36f0a-145">style</span><span class="sxs-lookup"><span data-stu-id="36f0a-145">style</span></span>|<span data-ttu-id="36f0a-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36f0a-146">string</span></span>|<span data-ttu-id="36f0a-147">Valor da constante que representa o estilo de Tabela.</span><span class="sxs-lookup"><span data-stu-id="36f0a-147">Constant value that represents the Table style.</span></span> <span data-ttu-id="36f0a-148">Os valores possíveis são: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="36f0a-148">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="36f0a-149">Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.</span><span class="sxs-lookup"><span data-stu-id="36f0a-149">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="36f0a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="36f0a-150">Response</span></span>

<span data-ttu-id="36f0a-151">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbooktable](../resources/table.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36f0a-151">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36f0a-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36f0a-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36f0a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36f0a-153">Request</span></span>
<span data-ttu-id="36f0a-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36f0a-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36f0a-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="36f0a-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36f0a-156">C#</span><span class="sxs-lookup"><span data-stu-id="36f0a-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36f0a-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36f0a-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36f0a-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36f0a-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36f0a-159">Java</span><span class="sxs-lookup"><span data-stu-id="36f0a-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36f0a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="36f0a-160">Response</span></span>
<span data-ttu-id="36f0a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36f0a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
