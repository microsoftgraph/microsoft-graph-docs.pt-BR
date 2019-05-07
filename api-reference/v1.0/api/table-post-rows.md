---
title: Criar TableRow
description: 'Adiciona linhas ao final da tabela. Observe que a API pode aceitar vários dados de linhas usando essa API. A adição de uma linha por vez pode levar à degradação de desempenho. A abordagem recomendada seria colocar as linhas em lote em uma única chamada em vez de fazer uma única inserção de linha. Para obter melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute uma operação de adição de linhas únicas. Experimente o número de linhas para determinar o número ideal de linhas a serem usadas em uma única chamada de API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5421d684c15da9ff684732d60422a73714bf7d8f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602790"
---
# <a name="create-tablerow"></a><span data-ttu-id="0d618-108">Criar TableRow</span><span class="sxs-lookup"><span data-stu-id="0d618-108">Create TableRow</span></span>

<span data-ttu-id="0d618-109">Adiciona linhas ao final da tabela.</span><span class="sxs-lookup"><span data-stu-id="0d618-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="0d618-110">Observe que a API pode aceitar vários dados de linhas usando essa API.</span><span class="sxs-lookup"><span data-stu-id="0d618-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="0d618-111">A adição de uma linha por vez pode levar à degradação de desempenho.</span><span class="sxs-lookup"><span data-stu-id="0d618-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="0d618-112">A abordagem recomendada seria colocar as linhas em lote em uma única chamada em vez de fazer uma única inserção de linha.</span><span class="sxs-lookup"><span data-stu-id="0d618-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="0d618-113">Para obter melhores resultados, colete as linhas a serem inseridas no lado do aplicativo e execute uma operação de adição de linhas únicas.</span><span class="sxs-lookup"><span data-stu-id="0d618-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="0d618-114">Experimente o número de linhas para determinar o número ideal de linhas a serem usadas em uma única chamada de API.</span><span class="sxs-lookup"><span data-stu-id="0d618-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="0d618-115">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="0d618-115">Error Handling</span></span>

<span data-ttu-id="0d618-116">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="0d618-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="0d618-117">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d618-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d618-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d618-118">Permissions</span></span>
<span data-ttu-id="0d618-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d618-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d618-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d618-121">Permission type</span></span>      | <span data-ttu-id="0d618-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d618-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d618-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d618-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0d618-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d618-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0d618-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d618-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d618-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d618-126">Not supported.</span></span>    |
|<span data-ttu-id="0d618-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d618-127">Application</span></span> | <span data-ttu-id="0d618-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d618-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d618-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d618-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="0d618-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d618-130">Request headers</span></span>
| <span data-ttu-id="0d618-131">Nome</span><span class="sxs-lookup"><span data-stu-id="0d618-131">Name</span></span>       | <span data-ttu-id="0d618-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d618-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d618-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d618-133">Authorization</span></span>  | <span data-ttu-id="0d618-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d618-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d618-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0d618-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="0d618-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d618-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d618-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d618-139">Request body</span></span>
<span data-ttu-id="0d618-140">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d618-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0d618-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0d618-141">Parameter</span></span>    | <span data-ttu-id="0d618-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d618-142">Type</span></span>   |<span data-ttu-id="0d618-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d618-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d618-144">index</span><span class="sxs-lookup"><span data-stu-id="0d618-144">index</span></span>|<span data-ttu-id="0d618-145">number</span><span class="sxs-lookup"><span data-stu-id="0d618-145">number</span></span>|<span data-ttu-id="0d618-p107">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="0d618-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="0d618-151">values</span><span class="sxs-lookup"><span data-stu-id="0d618-151">values</span></span>|<span data-ttu-id="0d618-152">Json</span><span class="sxs-lookup"><span data-stu-id="0d618-152">Json</span></span>|<span data-ttu-id="0d618-153">Uma matriz bidimensional de valores não formatados das linhas da tabela (Boolean ou String ou número).</span><span class="sxs-lookup"><span data-stu-id="0d618-153">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="0d618-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d618-154">Response</span></span>

<span data-ttu-id="0d618-155">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d618-155">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d618-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d618-156">Example</span></span>
<span data-ttu-id="0d618-157">Neste exemplo, duas linhas de dados são inseridas no final da tabela.</span><span class="sxs-lookup"><span data-stu-id="0d618-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="0d618-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d618-158">Request</span></span>
<span data-ttu-id="0d618-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d618-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
##### <a name="response"></a><span data-ttu-id="0d618-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d618-160">Response</span></span>
<span data-ttu-id="0d618-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d618-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d618-164">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0d618-164">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d618-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d618-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablerowcollection_add-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-post-rows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/table-post-rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table-post-rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->
