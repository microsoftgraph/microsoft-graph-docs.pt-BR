---
title: 'ChartLineFormat: clear'
description: Limpe a formatação da linha de um elemento do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 812850e0def2cecafa19a25605d37d403d2ab51d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521380"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="db351-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="db351-103">ChartLineFormat: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db351-104">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="db351-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="db351-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db351-105">Permissions</span></span>
<span data-ttu-id="db351-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db351-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db351-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db351-108">Permission type</span></span>      | <span data-ttu-id="db351-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db351-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db351-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db351-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db351-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db351-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db351-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db351-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db351-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db351-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db351-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db351-114">Application</span></span> | <span data-ttu-id="db351-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db351-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db351-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db351-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="db351-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db351-117">Request headers</span></span>
| <span data-ttu-id="db351-118">Nome</span><span class="sxs-lookup"><span data-stu-id="db351-118">Name</span></span>       | <span data-ttu-id="db351-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="db351-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db351-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="db351-120">Authorization</span></span>  | <span data-ttu-id="db351-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db351-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db351-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db351-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="db351-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="db351-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db351-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db351-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="db351-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="db351-127">Response</span></span>

<span data-ttu-id="db351-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db351-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db351-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db351-130">Example</span></span>
<span data-ttu-id="db351-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="db351-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db351-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db351-132">Request</span></span>
<span data-ttu-id="db351-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db351-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="db351-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="db351-134">Response</span></span>
<span data-ttu-id="db351-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db351-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartlineformat-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
