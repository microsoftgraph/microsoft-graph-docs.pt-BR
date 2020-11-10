---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f54fd06feb33b2324550ac3ce777bb610923d527
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977573"
---
# <a name="create-table"></a><span data-ttu-id="195fe-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="195fe-103">Create table</span></span>

<span data-ttu-id="195fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="195fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="195fe-105">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="195fe-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="195fe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="195fe-106">Permissions</span></span>
<span data-ttu-id="195fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="195fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="195fe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="195fe-109">Permission type</span></span>      | <span data-ttu-id="195fe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="195fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="195fe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="195fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="195fe-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="195fe-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="195fe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="195fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="195fe-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="195fe-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="195fe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="195fe-115">Application</span></span> | <span data-ttu-id="195fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="195fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="195fe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="195fe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="195fe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="195fe-118">Request headers</span></span>
| <span data-ttu-id="195fe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="195fe-119">Name</span></span>       | <span data-ttu-id="195fe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="195fe-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="195fe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="195fe-121">Authorization</span></span>  | <span data-ttu-id="195fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="195fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="195fe-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="195fe-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="195fe-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="195fe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="195fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="195fe-127">Request body</span></span>
<span data-ttu-id="195fe-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="195fe-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="195fe-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="195fe-129">Parameter</span></span>           | <span data-ttu-id="195fe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="195fe-130">Type</span></span>      |<span data-ttu-id="195fe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="195fe-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="195fe-132">Endereço</span><span class="sxs-lookup"><span data-stu-id="195fe-132">Address</span></span>  | <span data-ttu-id="195fe-133">string</span><span class="sxs-lookup"><span data-stu-id="195fe-133">string</span></span>| <span data-ttu-id="195fe-134">Endereço do intervalo.</span><span class="sxs-lookup"><span data-stu-id="195fe-134">Range address.</span></span> <span data-ttu-id="195fe-135">Se você estiver chamando esta API fora do `worksheets/{id or name}/tables/add` caminho, não será necessário para o prefixo do nome da planilha no endereço.</span><span class="sxs-lookup"><span data-stu-id="195fe-135">If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address.</span></span> <span data-ttu-id="195fe-136">No entanto, se você estiver ligando para fora do `workbook/tables/add` caminho, forneça o nome da planilha na qual a tabela precisa ser criada (exemplo: `sheet1!A1:D4` )</span><span class="sxs-lookup"><span data-stu-id="195fe-136">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="195fe-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="195fe-137">hasHeaders</span></span>  | <span data-ttu-id="195fe-138">booliano</span><span class="sxs-lookup"><span data-stu-id="195fe-138">boolean</span></span>|<span data-ttu-id="195fe-139">Valor booliano que indica se o intervalo tem rótulos de coluna.</span><span class="sxs-lookup"><span data-stu-id="195fe-139">Boolean value that indicates whether the range has column labels.</span></span> <span data-ttu-id="195fe-140">Se a fonte não contiver cabeçalhos (ou seja,.</span><span class="sxs-lookup"><span data-stu-id="195fe-140">If the source does not contain headers (i.e,.</span></span> <span data-ttu-id="195fe-141">Quando essa propriedade for definida como false, o Excel gerará automaticamente o cabeçalho deslocando os dados de uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="195fe-141">when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="195fe-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="195fe-142">Response</span></span>

<span data-ttu-id="195fe-143">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [workbooktable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="195fe-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="195fe-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="195fe-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="195fe-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="195fe-145">Request</span></span>
<span data-ttu-id="195fe-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="195fe-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="195fe-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="195fe-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="195fe-148">C#</span><span class="sxs-lookup"><span data-stu-id="195fe-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-workbook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="195fe-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="195fe-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-workbook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="195fe-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="195fe-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-workbook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="195fe-151">Java</span><span class="sxs-lookup"><span data-stu-id="195fe-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-workbook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="195fe-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="195fe-152">Response</span></span>
<span data-ttu-id="195fe-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="195fe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


