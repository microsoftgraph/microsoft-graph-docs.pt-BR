---
title: 'TableCollection: add'
description: Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 017af4dde30e62deb25512cf8313b9975ac09c0a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271005"
---
# <a name="tablecollection-add"></a><span data-ttu-id="9dfe1-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="9dfe1-105">TableCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dfe1-p102">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="9dfe1-109">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="9dfe1-109">Error Handling</span></span>

<span data-ttu-id="9dfe1-110">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-110">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="9dfe1-111">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-111">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dfe1-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9dfe1-112">Permissions</span></span>
<span data-ttu-id="9dfe1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dfe1-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9dfe1-115">Permission type</span></span>      | <span data-ttu-id="9dfe1-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9dfe1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dfe1-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9dfe1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9dfe1-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dfe1-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9dfe1-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9dfe1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dfe1-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dfe1-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9dfe1-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dfe1-121">Application</span></span> | <span data-ttu-id="9dfe1-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dfe1-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dfe1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="9dfe1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfe1-124">Request headers</span></span>
| <span data-ttu-id="9dfe1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9dfe1-125">Name</span></span>       | <span data-ttu-id="9dfe1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dfe1-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dfe1-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dfe1-127">Authorization</span></span>  | <span data-ttu-id="9dfe1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9dfe1-130">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9dfe1-130">Workbook-Session-Id</span></span>  | <span data-ttu-id="9dfe1-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dfe1-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfe1-133">Request body</span></span>
<span data-ttu-id="9dfe1-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9dfe1-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9dfe1-135">Parameter</span></span>    | <span data-ttu-id="9dfe1-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dfe1-136">Type</span></span>   |<span data-ttu-id="9dfe1-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dfe1-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dfe1-138">address</span><span class="sxs-lookup"><span data-stu-id="9dfe1-138">address</span></span>|<span data-ttu-id="9dfe1-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dfe1-139">string</span></span>|<span data-ttu-id="9dfe1-p107">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="9dfe1-142">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="9dfe1-142">hasHeaders</span></span>|<span data-ttu-id="9dfe1-143">booliano</span><span class="sxs-lookup"><span data-stu-id="9dfe1-143">boolean</span></span>|<span data-ttu-id="9dfe1-p108">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="9dfe1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dfe1-147">Response</span></span>

<span data-ttu-id="9dfe1-148">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbooktable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-148">If successful, this method returns `200 OK` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dfe1-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9dfe1-149">Example</span></span>
<span data-ttu-id="9dfe1-150">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9dfe1-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfe1-151">Request</span></span>
<span data-ttu-id="9dfe1-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="9dfe1-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dfe1-153">Response</span></span>
<span data-ttu-id="9dfe1-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9dfe1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9dfe1-157">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9dfe1-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9dfe1-158">C#</span><span class="sxs-lookup"><span data-stu-id="9dfe1-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9dfe1-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="9dfe1-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9dfe1-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9dfe1-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
