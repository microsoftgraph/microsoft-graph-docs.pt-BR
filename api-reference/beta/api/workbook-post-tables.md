---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
ms.openlocfilehash: 75d4199b4c5cefcb17acccfedfb5c45a3f296de0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321620"
---
# <a name="create-table"></a><span data-ttu-id="aaaef-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="aaaef-103">Create table</span></span>

> <span data-ttu-id="aaaef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aaaef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaaef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aaaef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aaaef-106">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="aaaef-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="aaaef-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="aaaef-107">Permissions</span></span>
<span data-ttu-id="aaaef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaaef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaaef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaaef-110">Permission type</span></span>      | <span data-ttu-id="aaaef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aaaef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaaef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaaef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aaaef-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaaef-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aaaef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaaef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaaef-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaaef-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aaaef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaaef-116">Application</span></span> | <span data-ttu-id="aaaef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaaef-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaaef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaaef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="aaaef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaaef-119">Request headers</span></span>
| <span data-ttu-id="aaaef-120">Nome</span><span class="sxs-lookup"><span data-stu-id="aaaef-120">Name</span></span>       | <span data-ttu-id="aaaef-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaaef-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aaaef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaaef-122">Authorization</span></span>  | <span data-ttu-id="aaaef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaaef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aaaef-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aaaef-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="aaaef-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="aaaef-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaaef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaaef-128">Request body</span></span>
<span data-ttu-id="aaaef-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaaef-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aaaef-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aaaef-130">Parameter</span></span>           | <span data-ttu-id="aaaef-131">Type</span><span class="sxs-lookup"><span data-stu-id="aaaef-131">Type</span></span>      |<span data-ttu-id="aaaef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaaef-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="aaaef-133">Endereço</span><span class="sxs-lookup"><span data-stu-id="aaaef-133">Address</span></span>  | <span data-ttu-id="aaaef-134">string</span><span class="sxs-lookup"><span data-stu-id="aaaef-134">string</span></span>| <span data-ttu-id="aaaef-p105">Endereço do intervalo. Se você estiver chamando essa API fora do caminho `worksheets/{id or name}/tables/add`, não haverá necessidade do prefixo de nome da planilha no endereço. No entanto, se você a estiver chamando fora do caminho `workbook/tables/add`, forneça então o nome da planilha em que a tabela precisa ser criada (exemplo: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="aaaef-p105">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="aaaef-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="aaaef-138">hasHeaders</span></span>  | <span data-ttu-id="aaaef-139">booliano</span><span class="sxs-lookup"><span data-stu-id="aaaef-139">boolean</span></span>|<span data-ttu-id="aaaef-p106">O valor booliano que indica se o intervalo tem rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="aaaef-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="aaaef-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaaef-143">Response</span></span>

<span data-ttu-id="aaaef-144">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaaef-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaaef-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaaef-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aaaef-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaaef-146">Request</span></span>
<span data-ttu-id="aaaef-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaaef-147">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="aaaef-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaaef-148">Response</span></span>
<span data-ttu-id="aaaef-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaaef-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
