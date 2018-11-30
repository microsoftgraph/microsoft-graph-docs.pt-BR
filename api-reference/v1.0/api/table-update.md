---
title: Atualizar tabela
description: Atualize as propriedades do objeto de tabela.
ms.openlocfilehash: 0bf3979dcc056b6a32e9c4bb7c89bf3d6a7fab57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005267"
---
# <a name="update-table"></a><span data-ttu-id="97db7-103">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="97db7-103">Update table</span></span>

<span data-ttu-id="97db7-104">Atualize as propriedades do objeto de tabela.</span><span class="sxs-lookup"><span data-stu-id="97db7-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="97db7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97db7-105">Permissions</span></span>
<span data-ttu-id="97db7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97db7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97db7-108">Permission type</span></span>      | <span data-ttu-id="97db7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97db7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97db7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97db7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97db7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97db7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="97db7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97db7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97db7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97db7-113">Not supported.</span></span>    |
|<span data-ttu-id="97db7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97db7-114">Application</span></span> | <span data-ttu-id="97db7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97db7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97db7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97db7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="97db7-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="97db7-117">Optional request headers</span></span>
| <span data-ttu-id="97db7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="97db7-118">Name</span></span>       | <span data-ttu-id="97db7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="97db7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97db7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="97db7-120">Authorization</span></span>  | <span data-ttu-id="97db7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97db7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97db7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="97db7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="97db7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97db7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97db7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97db7-126">Request body</span></span>
<span data-ttu-id="97db7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="97db7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97db7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97db7-130">Property</span></span>     | <span data-ttu-id="97db7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97db7-131">Type</span></span>   |<span data-ttu-id="97db7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97db7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97db7-133">name</span><span class="sxs-lookup"><span data-stu-id="97db7-133">name</span></span>|<span data-ttu-id="97db7-134">string</span><span class="sxs-lookup"><span data-stu-id="97db7-134">string</span></span>|<span data-ttu-id="97db7-135">Nome da tabela.</span><span class="sxs-lookup"><span data-stu-id="97db7-135">Name of the table.</span></span>|
|<span data-ttu-id="97db7-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="97db7-136">showHeaders</span></span>|<span data-ttu-id="97db7-137">booliano</span><span class="sxs-lookup"><span data-stu-id="97db7-137">boolean</span></span>|<span data-ttu-id="97db7-p105">Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="97db7-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="97db7-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="97db7-140">showTotals</span></span>|<span data-ttu-id="97db7-141">booliano</span><span class="sxs-lookup"><span data-stu-id="97db7-141">boolean</span></span>|<span data-ttu-id="97db7-p106">Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.</span><span class="sxs-lookup"><span data-stu-id="97db7-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="97db7-144">style</span><span class="sxs-lookup"><span data-stu-id="97db7-144">style</span></span>|<span data-ttu-id="97db7-145">string</span><span class="sxs-lookup"><span data-stu-id="97db7-145">string</span></span>|<span data-ttu-id="97db7-146">Valor de constante que representa o estilo de tabela.</span><span class="sxs-lookup"><span data-stu-id="97db7-146">Constant value that represents the Table style.</span></span> <span data-ttu-id="97db7-147">Os valores possíveis são: TableStyleLight1 até o TableStyleLight21, TableStyleMedium1 até o TableStyleMedium28, TableStyleStyleDark1 até o TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="97db7-147">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="97db7-148">Um estilo personalizado de definidas pelo usuário presente na pasta de trabalho também pode ser especificado.</span><span class="sxs-lookup"><span data-stu-id="97db7-148">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="97db7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="97db7-149">Response</span></span>

<span data-ttu-id="97db7-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookTable](../resources/table.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97db7-150">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97db7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97db7-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97db7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97db7-152">Request</span></span>
<span data-ttu-id="97db7-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97db7-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="97db7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="97db7-154">Response</span></span>
<span data-ttu-id="97db7-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97db7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
