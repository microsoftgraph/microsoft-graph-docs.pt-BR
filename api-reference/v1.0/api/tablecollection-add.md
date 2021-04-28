---
title: 'TableCollection: add'
description: Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3e7304fd1e3d85a60ac9f14f66ace5c3e6adfe16
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051239"
---
# <a name="tablecollection-add"></a><span data-ttu-id="1fcef-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="1fcef-105">TableCollection: add</span></span>

<span data-ttu-id="1fcef-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fcef-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1fcef-p102">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="1fcef-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="1fcef-110">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="1fcef-110">Error Handling</span></span>

<span data-ttu-id="1fcef-111">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="1fcef-111">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="1fcef-112">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fcef-112">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fcef-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fcef-113">Permissions</span></span>
<span data-ttu-id="1fcef-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fcef-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fcef-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fcef-116">Permission type</span></span>      | <span data-ttu-id="1fcef-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fcef-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fcef-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fcef-118">Delegated (work or school account)</span></span> | <span data-ttu-id="1fcef-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fcef-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1fcef-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fcef-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fcef-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fcef-121">Not supported.</span></span>    |
|<span data-ttu-id="1fcef-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fcef-122">Application</span></span> | <span data-ttu-id="1fcef-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fcef-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fcef-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fcef-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/add
POST /me/drive/root:/{item-path}:/workbook/tables/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="1fcef-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcef-125">Request headers</span></span>
| <span data-ttu-id="1fcef-126">Nome</span><span class="sxs-lookup"><span data-stu-id="1fcef-126">Name</span></span>       | <span data-ttu-id="1fcef-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcef-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1fcef-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fcef-128">Authorization</span></span>  | <span data-ttu-id="1fcef-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fcef-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fcef-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1fcef-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="1fcef-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1fcef-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fcef-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcef-134">Request body</span></span>
<span data-ttu-id="1fcef-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fcef-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1fcef-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1fcef-136">Parameter</span></span>    | <span data-ttu-id="1fcef-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fcef-137">Type</span></span>   |<span data-ttu-id="1fcef-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcef-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fcef-139">address</span><span class="sxs-lookup"><span data-stu-id="1fcef-139">address</span></span>|<span data-ttu-id="1fcef-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fcef-140">string</span></span>|<span data-ttu-id="1fcef-p107">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="1fcef-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="1fcef-143">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="1fcef-143">hasHeaders</span></span>|<span data-ttu-id="1fcef-144">booliano</span><span class="sxs-lookup"><span data-stu-id="1fcef-144">boolean</span></span>|<span data-ttu-id="1fcef-p108">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="1fcef-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="1fcef-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fcef-148">Response</span></span>

<span data-ttu-id="1fcef-149">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fcef-149">If successful, this method returns `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fcef-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fcef-150">Example</span></span>
<span data-ttu-id="1fcef-151">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1fcef-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1fcef-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcef-152">Request</span></span>
<span data-ttu-id="1fcef-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fcef-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fcef-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fcef-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```
# <a name="c"></a>[<span data-ttu-id="1fcef-155">C#</span><span class="sxs-lookup"><span data-stu-id="1fcef-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fcef-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fcef-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fcef-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fcef-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fcef-158">Java</span><span class="sxs-lookup"><span data-stu-id="1fcef-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1fcef-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fcef-159">Response</span></span>
<span data-ttu-id="1fcef-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fcef-160">Here is an example of the response.</span></span> <span data-ttu-id="1fcef-161">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1fcef-161">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

