---
title: 'TableRowCollection: add'
description: 'Adiciona linhas ao final da tabela. Observe que a API pode aceitar dados de várias linhas usando essa API. Adicionar uma linha por vez pode levar à degradação do desempenho. A abordagem recomendada seria reunir as linhas em lotes em uma única chamada em vez de fazer a inserção de linha única. Para melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute a operação de adicionar linhas simples. Experimente o número de linhas para determinar o número ideal de linhas a ser usado em uma única chamada de API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a0df946f7c3b859213a99d20b002b73301b2f919
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050259"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="9979e-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="9979e-108">TableRowCollection: add</span></span>

<span data-ttu-id="9979e-109">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9979e-109">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9979e-110">Adiciona linhas ao final da tabela.</span><span class="sxs-lookup"><span data-stu-id="9979e-110">Adds rows to the end of the table.</span></span> <span data-ttu-id="9979e-111">Observe que a API pode aceitar dados de várias linhas usando essa API.</span><span class="sxs-lookup"><span data-stu-id="9979e-111">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="9979e-112">Adicionar uma linha por vez pode levar à degradação do desempenho.</span><span class="sxs-lookup"><span data-stu-id="9979e-112">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="9979e-113">A abordagem recomendada seria reunir as linhas em lotes em uma única chamada em vez de fazer a inserção de linha única.</span><span class="sxs-lookup"><span data-stu-id="9979e-113">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="9979e-114">Para melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute a operação de adicionar linhas simples.</span><span class="sxs-lookup"><span data-stu-id="9979e-114">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="9979e-115">Experimente o número de linhas para determinar o número ideal de linhas a ser usado em uma única chamada de API.</span><span class="sxs-lookup"><span data-stu-id="9979e-115">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="9979e-116">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="9979e-116">Error Handling</span></span>

<span data-ttu-id="9979e-117">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="9979e-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="9979e-118">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9979e-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="9979e-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="9979e-119">Permissions</span></span>
<span data-ttu-id="9979e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9979e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9979e-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9979e-122">Permission type</span></span>      | <span data-ttu-id="9979e-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9979e-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9979e-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9979e-124">Delegated (work or school account)</span></span> | <span data-ttu-id="9979e-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9979e-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9979e-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9979e-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9979e-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9979e-127">Not supported.</span></span>    |
|<span data-ttu-id="9979e-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9979e-128">Application</span></span> | <span data-ttu-id="9979e-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9979e-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9979e-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9979e-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="9979e-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9979e-131">Request headers</span></span>
| <span data-ttu-id="9979e-132">Nome</span><span class="sxs-lookup"><span data-stu-id="9979e-132">Name</span></span>       | <span data-ttu-id="9979e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9979e-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9979e-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="9979e-134">Authorization</span></span>  | <span data-ttu-id="9979e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9979e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9979e-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9979e-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="9979e-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9979e-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9979e-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9979e-140">Request body</span></span>
<span data-ttu-id="9979e-141">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9979e-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9979e-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9979e-142">Parameter</span></span>    | <span data-ttu-id="9979e-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="9979e-143">Type</span></span>   |<span data-ttu-id="9979e-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="9979e-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9979e-145">índice</span><span class="sxs-lookup"><span data-stu-id="9979e-145">index</span></span>|<span data-ttu-id="9979e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9979e-146">Int32</span></span>|<span data-ttu-id="9979e-p107">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="9979e-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="9979e-152">values</span><span class="sxs-lookup"><span data-stu-id="9979e-152">values</span></span>|<span data-ttu-id="9979e-153">Json</span><span class="sxs-lookup"><span data-stu-id="9979e-153">Json</span></span>|<span data-ttu-id="9979e-p108">Opcional. Uma matriz bidimensional de valores não formatados da linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="9979e-p108">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="9979e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9979e-156">Response</span></span>

<span data-ttu-id="9979e-157">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookTableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9979e-157">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9979e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9979e-158">Example</span></span>
<span data-ttu-id="9979e-159">Neste exemplo, duas linhas de dados são inseridas no final da tabela.</span><span class="sxs-lookup"><span data-stu-id="9979e-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="9979e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9979e-160">Request</span></span>
<span data-ttu-id="9979e-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9979e-161">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9979e-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="9979e-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="9979e-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9979e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9979e-164">C#</span><span class="sxs-lookup"><span data-stu-id="9979e-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9979e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9979e-165">Response</span></span>
<span data-ttu-id="9979e-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9979e-166">Here is an example of the response.</span></span> <span data-ttu-id="9979e-167">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9979e-167">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->

