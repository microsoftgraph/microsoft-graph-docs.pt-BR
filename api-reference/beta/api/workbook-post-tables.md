---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e8f2d10c36ec8e2737b77b69fec46a4dd65e50c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448505"
---
# <a name="create-table"></a><span data-ttu-id="a4639-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="a4639-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4639-104">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="a4639-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4639-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4639-105">Permissions</span></span>
<span data-ttu-id="a4639-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4639-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4639-108">Permission type</span></span>      | <span data-ttu-id="a4639-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4639-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4639-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4639-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4639-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4639-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a4639-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4639-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4639-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4639-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a4639-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4639-114">Application</span></span> | <span data-ttu-id="a4639-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4639-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4639-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4639-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="a4639-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4639-117">Request headers</span></span>
| <span data-ttu-id="a4639-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a4639-118">Name</span></span>       | <span data-ttu-id="a4639-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4639-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4639-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4639-120">Authorization</span></span>  | <span data-ttu-id="a4639-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4639-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4639-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a4639-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a4639-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4639-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4639-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4639-126">Request body</span></span>
<span data-ttu-id="a4639-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4639-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4639-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4639-128">Parameter</span></span>           | <span data-ttu-id="a4639-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4639-129">Type</span></span>      |<span data-ttu-id="a4639-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4639-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="a4639-131">Endereço</span><span class="sxs-lookup"><span data-stu-id="a4639-131">Address</span></span>  | <span data-ttu-id="a4639-132">string</span><span class="sxs-lookup"><span data-stu-id="a4639-132">string</span></span>| <span data-ttu-id="a4639-133">Endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="a4639-133">Range address.</span></span> <span data-ttu-id="a4639-134">Se você estiver chamando esta API fora do `worksheets/{id or name}/tables/add` caminho, não será necessário para o prefixo do nome da planilha no endereço.</span><span class="sxs-lookup"><span data-stu-id="a4639-134">If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address.</span></span> <span data-ttu-id="a4639-135">No entanto, se você estiver ligando para `workbook/tables/add` fora do caminho, forneça o nome da planilha na qual a tabela precisa ser criada (exemplo `sheet1!A1:D4`:)</span><span class="sxs-lookup"><span data-stu-id="a4639-135">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="a4639-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="a4639-136">hasHeaders</span></span>  | <span data-ttu-id="a4639-137">booliano</span><span class="sxs-lookup"><span data-stu-id="a4639-137">boolean</span></span>|<span data-ttu-id="a4639-138">Valor booliano que indica se o intervalo tem rótulos de coluna.</span><span class="sxs-lookup"><span data-stu-id="a4639-138">Boolean value that indicates whether the range has column labels.</span></span> <span data-ttu-id="a4639-139">Se a fonte não contiver cabeçalhos (ou seja,.</span><span class="sxs-lookup"><span data-stu-id="a4639-139">If the source does not contain headers (i.e,.</span></span> <span data-ttu-id="a4639-140">Quando essa propriedade for definida como false, o Excel gerará automaticamente o cabeçalho deslocando os dados de uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="a4639-140">when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="a4639-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4639-141">Response</span></span>

<span data-ttu-id="a4639-142">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [workbooktable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4639-142">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4639-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4639-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4639-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4639-144">Request</span></span>
<span data-ttu-id="a4639-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4639-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4639-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4639-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4639-147">C#</span><span class="sxs-lookup"><span data-stu-id="a4639-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-workbook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4639-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4639-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-workbook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4639-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a4639-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-workbook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4639-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4639-150">Response</span></span>
<span data-ttu-id="a4639-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4639-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
