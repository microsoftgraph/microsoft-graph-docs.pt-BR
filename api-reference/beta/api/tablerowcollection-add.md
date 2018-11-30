---
title: 'TableRowCollection: add'
description: 'Adiciona linhas até o final da tabela. Observe que a API pode aceitar os dados de várias linhas usando essa API. Adicionar uma linha por vez pode levar à redução de desempenho. A abordagem recomendada seria as linhas juntos em uma única chamada em vez de fazer a inserção de linha única de lote. Para obter melhores resultados, coletado linhas a ser inserido no lado do aplicativo e realizar linhas única Adicionar operação. Experimentar o número de linhas para determinar o número ideal de linhas para usar em única chamada de API. '
ms.openlocfilehash: 20f131737d51ff0fa09004a80d5d24c3b6673cc8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038312"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="14dc5-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="14dc5-108">TableRowCollection: add</span></span>

> <span data-ttu-id="14dc5-109">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="14dc5-109">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14dc5-110">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="14dc5-110">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14dc5-111">Adiciona linhas até o final da tabela.</span><span class="sxs-lookup"><span data-stu-id="14dc5-111">Adds rows to the end of the table.</span></span> <span data-ttu-id="14dc5-112">Observe que a API pode aceitar os dados de várias linhas usando essa API.</span><span class="sxs-lookup"><span data-stu-id="14dc5-112">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="14dc5-113">Adicionar uma linha por vez pode levar à redução de desempenho.</span><span class="sxs-lookup"><span data-stu-id="14dc5-113">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="14dc5-114">A abordagem recomendada seria as linhas juntos em uma única chamada em vez de fazer a inserção de linha única de lote.</span><span class="sxs-lookup"><span data-stu-id="14dc5-114">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="14dc5-115">Para obter melhores resultados, coletado linhas a ser inserido no lado do aplicativo e realizar linhas única Adicionar operação.</span><span class="sxs-lookup"><span data-stu-id="14dc5-115">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="14dc5-116">Experimentar o número de linhas para determinar o número ideal de linhas para usar em única chamada de API.</span><span class="sxs-lookup"><span data-stu-id="14dc5-116">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="14dc5-117">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="14dc5-117">Error Handling</span></span>

<span data-ttu-id="14dc5-118">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="14dc5-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="14dc5-119">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="14dc5-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="14dc5-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="14dc5-120">Permissions</span></span>
<span data-ttu-id="14dc5-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14dc5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14dc5-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14dc5-123">Permission type</span></span>      | <span data-ttu-id="14dc5-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14dc5-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14dc5-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14dc5-125">Delegated (work or school account)</span></span> | <span data-ttu-id="14dc5-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14dc5-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14dc5-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14dc5-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14dc5-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14dc5-128">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14dc5-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14dc5-129">Application</span></span> | <span data-ttu-id="14dc5-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14dc5-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14dc5-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14dc5-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="14dc5-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14dc5-132">Request headers</span></span>
| <span data-ttu-id="14dc5-133">Nome</span><span class="sxs-lookup"><span data-stu-id="14dc5-133">Name</span></span>       | <span data-ttu-id="14dc5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="14dc5-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="14dc5-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="14dc5-135">Authorization</span></span>  | <span data-ttu-id="14dc5-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14dc5-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14dc5-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="14dc5-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="14dc5-p107">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="14dc5-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14dc5-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14dc5-141">Request body</span></span>
<span data-ttu-id="14dc5-142">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14dc5-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14dc5-143">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="14dc5-143">Parameter</span></span>    | <span data-ttu-id="14dc5-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="14dc5-144">Type</span></span>   |<span data-ttu-id="14dc5-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="14dc5-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14dc5-146">índice</span><span class="sxs-lookup"><span data-stu-id="14dc5-146">index</span></span>|<span data-ttu-id="14dc5-147">número</span><span class="sxs-lookup"><span data-stu-id="14dc5-147">number</span></span>|<span data-ttu-id="14dc5-p108">Opcional. Especifica a posição relativa da nova linha. Se for nulo, a adição ocorre no final. Todas as linhas abaixo da linha inserida serão deslocadas para baixo. Indexado com zero.</span><span class="sxs-lookup"><span data-stu-id="14dc5-p108">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="14dc5-153">values</span><span class="sxs-lookup"><span data-stu-id="14dc5-153">values</span></span>|<span data-ttu-id="14dc5-154">(booliano, cadeia de caracteres ou número)</span><span class="sxs-lookup"><span data-stu-id="14dc5-154">(boolean or string or number)</span></span>|<span data-ttu-id="14dc5-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14dc5-155">Optional.</span></span> <span data-ttu-id="14dc5-156">Uma matriz de 2-dimensional dos valores não formatados das linhas da tabela.</span><span class="sxs-lookup"><span data-stu-id="14dc5-156">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="14dc5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="14dc5-157">Response</span></span>

<span data-ttu-id="14dc5-158">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [TableRow](../resources/tablerow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14dc5-158">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14dc5-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14dc5-159">Example</span></span>
<span data-ttu-id="14dc5-160">Neste exemplo, duas linhas de dados são inseridas no fim da tabela.</span><span class="sxs-lookup"><span data-stu-id="14dc5-160">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="14dc5-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14dc5-161">Request</span></span>
<span data-ttu-id="14dc5-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14dc5-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="14dc5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="14dc5-163">Response</span></span>
<span data-ttu-id="14dc5-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14dc5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->
