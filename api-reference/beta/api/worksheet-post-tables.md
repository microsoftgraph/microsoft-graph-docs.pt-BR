---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 133b57c66cd0333c4dec1cd37895369749889bbb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050700"
---
# <a name="create-table"></a><span data-ttu-id="a871f-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="a871f-103">Create table</span></span>

<span data-ttu-id="a871f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a871f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a871f-105">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="a871f-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="a871f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a871f-106">Permissions</span></span>
<span data-ttu-id="a871f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a871f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a871f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a871f-109">Permission type</span></span>      | <span data-ttu-id="a871f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a871f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a871f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a871f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a871f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a871f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a871f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a871f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a871f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a871f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a871f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a871f-115">Application</span></span> | <span data-ttu-id="a871f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a871f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a871f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a871f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="a871f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a871f-118">Request headers</span></span>
| <span data-ttu-id="a871f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a871f-119">Name</span></span>       | <span data-ttu-id="a871f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a871f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a871f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a871f-121">Authorization</span></span>  | <span data-ttu-id="a871f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a871f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a871f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a871f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a871f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a871f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a871f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a871f-127">Request body</span></span>
<span data-ttu-id="a871f-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a871f-128">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="a871f-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a871f-129">Parameter</span></span>       | <span data-ttu-id="a871f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a871f-130">Type</span></span>|<span data-ttu-id="a871f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a871f-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="a871f-132">Endereço</span><span class="sxs-lookup"><span data-stu-id="a871f-132">Address</span></span>  | <span data-ttu-id="a871f-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a871f-133">string</span></span>| <span data-ttu-id="a871f-134">Endereço de intervalo.</span><span class="sxs-lookup"><span data-stu-id="a871f-134">Range address.</span></span> <span data-ttu-id="a871f-135">Se você estiver chamando essa API fora do caminho, não há necessidade de dar suporte ao prefixo de nome da `worksheets/{id|name}/tables/add` planilha no endereço.</span><span class="sxs-lookup"><span data-stu-id="a871f-135">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="a871f-136">No entanto, se você estiver chamando isso fora do caminho, então fornece o nome da planilha no qual a tabela precisa `workbook/tables/add` ser criada (exemplo: `sheet1!A1:D4` )</span><span class="sxs-lookup"><span data-stu-id="a871f-136">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="a871f-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="a871f-137">hasHeaders</span></span>  | <span data-ttu-id="a871f-138">booliano</span><span class="sxs-lookup"><span data-stu-id="a871f-138">boolean</span></span>|<span data-ttu-id="a871f-139">Valor booleano que indica se o intervalo tem rótulos de coluna.</span><span class="sxs-lookup"><span data-stu-id="a871f-139">Boolean value that indicates whether the range has column labels.</span></span> <span data-ttu-id="a871f-140">Se a origem não contém os headers (ou seja,</span><span class="sxs-lookup"><span data-stu-id="a871f-140">If the source does not contain headers (i.e,.</span></span> <span data-ttu-id="a871f-141">quando essa propriedade for definida como false), Excel gerará automaticamente o header deslocando os dados para baixo por uma linha.</span><span class="sxs-lookup"><span data-stu-id="a871f-141">when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="a871f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a871f-142">Response</span></span>

<span data-ttu-id="a871f-143">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [workbookTable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a871f-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a871f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a871f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a871f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a871f-145">Request</span></span>
<span data-ttu-id="a871f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a871f-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a871f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="a871f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
# <a name="c"></a>[<span data-ttu-id="a871f-148">C#</span><span class="sxs-lookup"><span data-stu-id="a871f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a871f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a871f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a871f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a871f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a871f-151">Java</span><span class="sxs-lookup"><span data-stu-id="a871f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a871f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a871f-152">Response</span></span>
<span data-ttu-id="a871f-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a871f-153">Here is an example of the response.</span></span> <span data-ttu-id="a871f-154">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a871f-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


