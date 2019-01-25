---
title: Criar tabela
description: Use essa API para criar uma nova tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 649fb5848a7c30908a87d8ea643aefa19ca5623e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516368"
---
# <a name="create-table"></a><span data-ttu-id="86173-103">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="86173-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86173-104">Use essa API para criar uma nova tabela.</span><span class="sxs-lookup"><span data-stu-id="86173-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="86173-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86173-105">Permissions</span></span>
<span data-ttu-id="86173-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86173-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86173-108">Permission type</span></span>      | <span data-ttu-id="86173-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86173-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86173-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86173-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86173-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86173-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86173-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86173-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86173-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86173-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86173-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86173-114">Application</span></span> | <span data-ttu-id="86173-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86173-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86173-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86173-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="86173-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86173-117">Request headers</span></span>
| <span data-ttu-id="86173-118">Nome</span><span class="sxs-lookup"><span data-stu-id="86173-118">Name</span></span>       | <span data-ttu-id="86173-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="86173-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="86173-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="86173-120">Authorization</span></span>  | <span data-ttu-id="86173-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86173-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86173-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="86173-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="86173-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="86173-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86173-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86173-126">Request body</span></span>
<span data-ttu-id="86173-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86173-127">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="86173-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86173-128">Parameter</span></span>       | <span data-ttu-id="86173-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="86173-129">Type</span></span>|<span data-ttu-id="86173-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="86173-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="86173-131">Endereço</span><span class="sxs-lookup"><span data-stu-id="86173-131">Address</span></span>  | <span data-ttu-id="86173-132">string</span><span class="sxs-lookup"><span data-stu-id="86173-132">string</span></span>| <span data-ttu-id="86173-p104">Intervalo de endereço. Se você estiver retirando essa API de \`worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="86173-p104">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="86173-135">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span><span class="sxs-lookup"><span data-stu-id="86173-135">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="86173-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="86173-136">hasHeaders</span></span>  | <span data-ttu-id="86173-137">booliano</span><span class="sxs-lookup"><span data-stu-id="86173-137">boolean</span></span>|<span data-ttu-id="86173-p105">O valor booliano que indica se o intervalo tem rótulos de coluna. Se a origem não contiver cabeçalhos (ou seja, quando essa propriedade estiver definida como falso), o Excel gerará automaticamente um cabeçalho, deslocando os dados uma linha para baixo.</span><span class="sxs-lookup"><span data-stu-id="86173-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="86173-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="86173-141">Response</span></span>

<span data-ttu-id="86173-142">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Table](../resources/table.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86173-142">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86173-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86173-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86173-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86173-144">Request</span></span>
<span data-ttu-id="86173-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86173-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="86173-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="86173-146">Response</span></span>
<span data-ttu-id="86173-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86173-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-post-tables.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
