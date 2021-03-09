---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d399b86863fcf7ae95dd1bd9f65f72c45abbf4fe
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578189"
---
# <a name="create-table"></a><span data-ttu-id="65d07-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="65d07-103">Create table</span></span>

<span data-ttu-id="65d07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65d07-105">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="65d07-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="65d07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65d07-106">Permissions</span></span>
<span data-ttu-id="65d07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65d07-109">Permission type</span></span>      | <span data-ttu-id="65d07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65d07-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65d07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65d07-111">Delegated (work or school account)</span></span> | <span data-ttu-id="65d07-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65d07-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="65d07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65d07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d07-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65d07-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="65d07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65d07-115">Application</span></span> | <span data-ttu-id="65d07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65d07-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65d07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65d07-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="65d07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65d07-118">Request headers</span></span>
| <span data-ttu-id="65d07-119">Nome</span><span class="sxs-lookup"><span data-stu-id="65d07-119">Name</span></span>       | <span data-ttu-id="65d07-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="65d07-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65d07-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="65d07-121">Authorization</span></span>  | <span data-ttu-id="65d07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65d07-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65d07-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="65d07-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="65d07-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="65d07-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65d07-127">Request body</span></span>
<span data-ttu-id="65d07-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65d07-128">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="65d07-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="65d07-129">Parameter</span></span>       | <span data-ttu-id="65d07-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="65d07-130">Type</span></span>|<span data-ttu-id="65d07-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="65d07-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="65d07-132">Endereço</span><span class="sxs-lookup"><span data-stu-id="65d07-132">Address</span></span>  | <span data-ttu-id="65d07-133">string</span><span class="sxs-lookup"><span data-stu-id="65d07-133">string</span></span>| <span data-ttu-id="65d07-134">Endereço de intervalo.</span><span class="sxs-lookup"><span data-stu-id="65d07-134">Range address.</span></span> <span data-ttu-id="65d07-135">Se você estiver chamando essa API fora do caminho, não há necessidade de dar suporte ao prefixo de nome da `worksheets/{id|name}/tables/add` planilha no endereço.</span><span class="sxs-lookup"><span data-stu-id="65d07-135">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="65d07-136">No entanto, se você estiver chamando isso fora do caminho, então fornece o nome da planilha no qual a tabela precisa `workbook/tables/add` ser criada (exemplo: `sheet1!A1:D4` )</span><span class="sxs-lookup"><span data-stu-id="65d07-136">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="65d07-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="65d07-137">hasHeaders</span></span>  | <span data-ttu-id="65d07-138">booliano</span><span class="sxs-lookup"><span data-stu-id="65d07-138">boolean</span></span>|<span data-ttu-id="65d07-139">Valor booleano que indica se o intervalo tem rótulos de coluna.</span><span class="sxs-lookup"><span data-stu-id="65d07-139">Boolean value that indicates whether the range has column labels.</span></span> <span data-ttu-id="65d07-140">Se a origem não contém os headers (ou seja,</span><span class="sxs-lookup"><span data-stu-id="65d07-140">If the source does not contain headers (i.e,.</span></span> <span data-ttu-id="65d07-141">quando essa propriedade for definida como false), o Excel gerará automaticamente o header deslocando os dados para baixo por uma linha.</span><span class="sxs-lookup"><span data-stu-id="65d07-141">when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="65d07-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="65d07-142">Response</span></span>

<span data-ttu-id="65d07-143">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [workbookTable](../resources/workbooktable.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65d07-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65d07-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65d07-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65d07-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65d07-145">Request</span></span>
<span data-ttu-id="65d07-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65d07-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65d07-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="65d07-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="65d07-148">C#</span><span class="sxs-lookup"><span data-stu-id="65d07-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65d07-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65d07-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65d07-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65d07-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65d07-151">Java</span><span class="sxs-lookup"><span data-stu-id="65d07-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="65d07-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="65d07-152">Response</span></span>
<span data-ttu-id="65d07-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65d07-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


