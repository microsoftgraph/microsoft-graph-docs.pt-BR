---
title: 'Range: EntireColumn'
description: Obtém um objeto que representa toda a coluna do intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b97bf5f5b4e1f2f5ac95bf375608b831b7367328
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507597"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="ae0ec-103">Range: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="ae0ec-103">Range: EntireColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae0ec-104">Obtém um objeto que representa toda a coluna do intervalo.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-104">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae0ec-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae0ec-105">Permissions</span></span>
<span data-ttu-id="ae0ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae0ec-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae0ec-108">Permission type</span></span>      | <span data-ttu-id="ae0ec-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae0ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae0ec-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae0ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae0ec-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae0ec-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae0ec-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae0ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae0ec-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae0ec-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae0ec-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae0ec-114">Application</span></span> | <span data-ttu-id="ae0ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae0ec-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae0ec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/EntireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireColumn

```
## <a name="request-headers"></a><span data-ttu-id="ae0ec-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae0ec-117">Request headers</span></span>
| <span data-ttu-id="ae0ec-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ae0ec-118">Name</span></span>       | <span data-ttu-id="ae0ec-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae0ec-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae0ec-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae0ec-120">Authorization</span></span>  | <span data-ttu-id="ae0ec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae0ec-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae0ec-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae0ec-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae0ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae0ec-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ae0ec-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae0ec-127">Response</span></span>

<span data-ttu-id="ae0ec-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae0ec-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae0ec-129">Example</span></span>
<span data-ttu-id="ae0ec-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae0ec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae0ec-131">Request</span></span>
<span data-ttu-id="ae0ec-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/EntireColumn
```

##### <a name="response"></a><span data-ttu-id="ae0ec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae0ec-133">Response</span></span>
<span data-ttu-id="ae0ec-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae0ec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-entirecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
