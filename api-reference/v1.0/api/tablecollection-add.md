---
title: 'TableCollection: add'
description: Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0ef87e1a251ffd65754d9d949af26468b3daed9c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575900"
---
# <a name="tablecollection-add"></a><span data-ttu-id="7351b-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="7351b-105">TableCollection: add</span></span>

<span data-ttu-id="7351b-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7351b-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7351b-p102">Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="7351b-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="7351b-110">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="7351b-110">Error Handling</span></span>

<span data-ttu-id="7351b-111">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="7351b-111">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="7351b-112">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7351b-112">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="7351b-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="7351b-113">Permissions</span></span>
<span data-ttu-id="7351b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7351b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7351b-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7351b-116">Permission type</span></span>      | <span data-ttu-id="7351b-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7351b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7351b-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7351b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7351b-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7351b-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7351b-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7351b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7351b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7351b-121">Not supported.</span></span>    |
|<span data-ttu-id="7351b-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7351b-122">Application</span></span> | <span data-ttu-id="7351b-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7351b-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7351b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7351b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/add
POST /me/drive/root:/{item-path}:/workbook/tables/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="7351b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7351b-125">Request headers</span></span>
| <span data-ttu-id="7351b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="7351b-126">Name</span></span>       | <span data-ttu-id="7351b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="7351b-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7351b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="7351b-128">Authorization</span></span>  | <span data-ttu-id="7351b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7351b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7351b-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7351b-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="7351b-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7351b-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7351b-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7351b-134">Request body</span></span>
<span data-ttu-id="7351b-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7351b-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7351b-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7351b-136">Parameter</span></span>    | <span data-ttu-id="7351b-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="7351b-137">Type</span></span>   |<span data-ttu-id="7351b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7351b-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7351b-139">address</span><span class="sxs-lookup"><span data-stu-id="7351b-139">address</span></span>|<span data-ttu-id="7351b-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7351b-140">string</span></span>|<span data-ttu-id="7351b-p107">Endereço ou nome do objeto de intervalo que representa a fonte de dados. Se o endereço não contiver o nome de uma planilha, a folha ativa no momento será usada.</span><span class="sxs-lookup"><span data-stu-id="7351b-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="7351b-143">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="7351b-143">hasHeaders</span></span>|<span data-ttu-id="7351b-144">booliano</span><span class="sxs-lookup"><span data-stu-id="7351b-144">boolean</span></span>|<span data-ttu-id="7351b-p108">Valor booliano que indica se os dados que estão sendo importados têm rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="7351b-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="7351b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7351b-148">Response</span></span>

<span data-ttu-id="7351b-149">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7351b-149">If successful, this method returns `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7351b-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7351b-150">Example</span></span>
<span data-ttu-id="7351b-151">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7351b-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7351b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7351b-152">Request</span></span>
<span data-ttu-id="7351b-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7351b-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7351b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="7351b-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7351b-155">C#</span><span class="sxs-lookup"><span data-stu-id="7351b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7351b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7351b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7351b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7351b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7351b-158">Java</span><span class="sxs-lookup"><span data-stu-id="7351b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7351b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7351b-159">Response</span></span>
<span data-ttu-id="7351b-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7351b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

