---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 48da6649d65dfb8db15986b7e2f95e1342edcf42
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054277"
---
# <a name="create-table"></a><span data-ttu-id="c372d-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="c372d-103">Create table</span></span>

<span data-ttu-id="c372d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c372d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c372d-105">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="c372d-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c372d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c372d-106">Permissions</span></span>
<span data-ttu-id="c372d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c372d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c372d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c372d-109">Permission type</span></span>      | <span data-ttu-id="c372d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c372d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c372d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c372d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c372d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c372d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c372d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c372d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c372d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c372d-114">Not supported.</span></span>    |
|<span data-ttu-id="c372d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c372d-115">Application</span></span> | <span data-ttu-id="c372d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c372d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c372d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c372d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{table-id}/add
POST /me/drive/root:/{item-path}:/workbook/tables/{table-id}/add

```
## <a name="request-headers"></a><span data-ttu-id="c372d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c372d-118">Request headers</span></span>
| <span data-ttu-id="c372d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c372d-119">Name</span></span>       | <span data-ttu-id="c372d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c372d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c372d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c372d-121">Authorization</span></span>  | <span data-ttu-id="c372d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c372d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c372d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c372d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c372d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c372d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c372d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c372d-127">Request body</span></span>
<span data-ttu-id="c372d-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c372d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c372d-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c372d-129">Parameter</span></span>           | <span data-ttu-id="c372d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c372d-130">Type</span></span>      |<span data-ttu-id="c372d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c372d-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="c372d-132">Endereço</span><span class="sxs-lookup"><span data-stu-id="c372d-132">Address</span></span>  | <span data-ttu-id="c372d-133">string</span><span class="sxs-lookup"><span data-stu-id="c372d-133">string</span></span>| <span data-ttu-id="c372d-134">Endereço de intervalo.</span><span class="sxs-lookup"><span data-stu-id="c372d-134">Range address.</span></span> <span data-ttu-id="c372d-135">Se você estiver chamando essa API fora do caminho, não é necessário para prefixo de nome de `worksheets/{id or name}/tables/add` planilha no endereço.</span><span class="sxs-lookup"><span data-stu-id="c372d-135">If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address.</span></span> <span data-ttu-id="c372d-136">No entanto, se você estiver chamando isso fora do caminho, então fornece o nome da planilha no qual a tabela precisa `workbook/tables/add` ser criada (exemplo: `sheet1!A1:D4` )</span><span class="sxs-lookup"><span data-stu-id="c372d-136">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="c372d-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="c372d-137">hasHeaders</span></span>  | <span data-ttu-id="c372d-138">booliano</span><span class="sxs-lookup"><span data-stu-id="c372d-138">boolean</span></span>|<span data-ttu-id="c372d-139">Valor booleano que indica se o intervalo tem rótulos de coluna.</span><span class="sxs-lookup"><span data-stu-id="c372d-139">Boolean value that indicates whether the range has column labels.</span></span> <span data-ttu-id="c372d-140">Se a origem não contém os headers (ou seja,</span><span class="sxs-lookup"><span data-stu-id="c372d-140">If the source does not contain headers (i.e,.</span></span> <span data-ttu-id="c372d-141">quando essa propriedade for definida como false), Excel gerará automaticamente o header deslocando os dados para baixo por uma linha.</span><span class="sxs-lookup"><span data-stu-id="c372d-141">when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="c372d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c372d-142">Response</span></span>

<span data-ttu-id="c372d-143">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [WorkbookTable](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c372d-143">If successful, this method returns `201 Created` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c372d-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c372d-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c372d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c372d-145">Request</span></span>
<span data-ttu-id="c372d-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c372d-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{table-id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="c372d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c372d-147">Response</span></span>
<span data-ttu-id="c372d-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c372d-148">Here is an example of the response.</span></span> <span data-ttu-id="c372d-149">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c372d-149">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

