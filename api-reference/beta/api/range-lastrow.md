---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f6ed391f1158b6b9253827c52c50a0b197e31a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546197"
---
# <a name="range-lastrow"></a><span data-ttu-id="ead6b-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="ead6b-103">Range: LastRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ead6b-p101">Obtém a última linha do intervalo. Por exemplo, a última linha de "B2:D5" é "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="ead6b-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="ead6b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ead6b-106">Permissions</span></span>
<span data-ttu-id="ead6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ead6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ead6b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ead6b-109">Permission type</span></span>      | <span data-ttu-id="ead6b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ead6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ead6b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ead6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ead6b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ead6b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ead6b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ead6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ead6b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ead6b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ead6b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ead6b-115">Application</span></span> | <span data-ttu-id="ead6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ead6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ead6b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ead6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="ead6b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ead6b-118">Request headers</span></span>
| <span data-ttu-id="ead6b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ead6b-119">Name</span></span>       | <span data-ttu-id="ead6b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead6b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ead6b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ead6b-121">Authorization</span></span>  | <span data-ttu-id="ead6b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ead6b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ead6b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ead6b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ead6b-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ead6b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ead6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ead6b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ead6b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead6b-128">Response</span></span>

<span data-ttu-id="ead6b-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ead6b-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ead6b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ead6b-130">Example</span></span>
<span data-ttu-id="ead6b-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ead6b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ead6b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ead6b-132">Request</span></span>
<span data-ttu-id="ead6b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ead6b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="ead6b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead6b-134">Response</span></span>
<span data-ttu-id="ead6b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ead6b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
