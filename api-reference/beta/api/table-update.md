---
title: Atualizar tabela
description: Atualize as propriedades do objeto de tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b056a4e2255d4f3627673cb93865ca521947d689
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574954"
---
# <a name="update-table"></a><span data-ttu-id="3ae02-103">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="3ae02-103">Update table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ae02-104">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="3ae02-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ae02-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ae02-105">Permissions</span></span>
<span data-ttu-id="3ae02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ae02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ae02-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ae02-108">Permission type</span></span>      | <span data-ttu-id="3ae02-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ae02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ae02-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ae02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ae02-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ae02-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3ae02-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ae02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ae02-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ae02-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3ae02-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ae02-114">Application</span></span> | <span data-ttu-id="3ae02-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ae02-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ae02-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ae02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3ae02-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3ae02-117">Optional request headers</span></span>
| <span data-ttu-id="3ae02-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3ae02-118">Name</span></span>       | <span data-ttu-id="3ae02-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ae02-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3ae02-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ae02-120">Authorization</span></span>  | <span data-ttu-id="3ae02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ae02-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3ae02-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3ae02-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ae02-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae02-126">Request body</span></span>
<span data-ttu-id="3ae02-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3ae02-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ae02-130">Property</span></span>     | <span data-ttu-id="3ae02-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ae02-131">Type</span></span>   |<span data-ttu-id="3ae02-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ae02-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ae02-133">name</span><span class="sxs-lookup"><span data-stu-id="3ae02-133">name</span></span>|<span data-ttu-id="3ae02-134">string</span><span class="sxs-lookup"><span data-stu-id="3ae02-134">string</span></span>|<span data-ttu-id="3ae02-135">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="3ae02-135">Name of the table.</span></span>|
|<span data-ttu-id="3ae02-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="3ae02-136">showHeaders</span></span>|<span data-ttu-id="3ae02-137">booliano</span><span class="sxs-lookup"><span data-stu-id="3ae02-137">boolean</span></span>|<span data-ttu-id="3ae02-p105">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="3ae02-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="3ae02-140">showTotals</span></span>|<span data-ttu-id="3ae02-141">booliano</span><span class="sxs-lookup"><span data-stu-id="3ae02-141">boolean</span></span>|<span data-ttu-id="3ae02-p106">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="3ae02-144">style</span><span class="sxs-lookup"><span data-stu-id="3ae02-144">style</span></span>|<span data-ttu-id="3ae02-145">string</span><span class="sxs-lookup"><span data-stu-id="3ae02-145">string</span></span>|<span data-ttu-id="3ae02-p107">Valor da constante que representa o estilo de Tabela. Os valores possíveis são: TableStyleLight1 a TableStyleLight21, TableStyleMedium1 a TableStyleMedium28, TableStyleStyleDark1 a TableStyleStyleDark11. Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p107">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="3ae02-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ae02-149">Response</span></span>

<span data-ttu-id="3ae02-150">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Table](../resources/table.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ae02-150">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ae02-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ae02-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ae02-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ae02-152">Request</span></span>
<span data-ttu-id="3ae02-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ae02-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="3ae02-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ae02-154">Response</span></span>
<span data-ttu-id="3ae02-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ae02-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
