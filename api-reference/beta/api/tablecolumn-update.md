---
title: Atualizar tablecolumn
description: Atualize as propriedades do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1287cb8c7c8e9b477d1e103a1dc845cbb37b3b87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521401"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="cbe83-103">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="cbe83-103">Update tablecolumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbe83-104">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="cbe83-104">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbe83-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbe83-105">Permissions</span></span>
<span data-ttu-id="cbe83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbe83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbe83-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbe83-108">Permission type</span></span>      | <span data-ttu-id="cbe83-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbe83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbe83-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbe83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbe83-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbe83-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbe83-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbe83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbe83-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbe83-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbe83-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbe83-114">Application</span></span> | <span data-ttu-id="cbe83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbe83-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbe83-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbe83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cbe83-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="cbe83-117">Optional request headers</span></span>
| <span data-ttu-id="cbe83-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cbe83-118">Name</span></span>       | <span data-ttu-id="cbe83-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbe83-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cbe83-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbe83-120">Authorization</span></span>  | <span data-ttu-id="cbe83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbe83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbe83-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cbe83-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cbe83-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cbe83-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbe83-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbe83-126">Request body</span></span>
<span data-ttu-id="cbe83-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cbe83-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cbe83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbe83-130">Property</span></span>     | <span data-ttu-id="cbe83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbe83-131">Type</span></span>   |<span data-ttu-id="cbe83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbe83-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbe83-133">values</span><span class="sxs-lookup"><span data-stu-id="cbe83-133">values</span></span>|<span data-ttu-id="cbe83-134">json</span><span class="sxs-lookup"><span data-stu-id="cbe83-134">json</span></span>|<span data-ttu-id="cbe83-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="cbe83-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="cbe83-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbe83-138">Response</span></span>

<span data-ttu-id="cbe83-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableColumn](../resources/tablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbe83-139">If successful, this method returns a `200 OK` response code and updated [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbe83-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbe83-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbe83-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbe83-141">Request</span></span>
<span data-ttu-id="cbe83-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbe83-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="cbe83-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbe83-143">Response</span></span>
<span data-ttu-id="cbe83-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbe83-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
