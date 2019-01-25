---
title: 'workbookPivotTable: refreshAll'
description: Atualiza a tabela dinâmica dentro de uma determinada planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 734a1fa6e11211ca29a7a53a815ff88ebdd35fb5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525420"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="07ac3-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="07ac3-103">workbookPivotTable: refreshAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07ac3-104">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="07ac3-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="07ac3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="07ac3-105">Permissions</span></span>
<span data-ttu-id="07ac3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07ac3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07ac3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07ac3-108">Permission type</span></span>      | <span data-ttu-id="07ac3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07ac3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07ac3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07ac3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07ac3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07ac3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07ac3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07ac3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07ac3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07ac3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07ac3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07ac3-114">Application</span></span> | <span data-ttu-id="07ac3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07ac3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07ac3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07ac3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="07ac3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07ac3-117">Request headers</span></span>
| <span data-ttu-id="07ac3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="07ac3-118">Name</span></span>       | <span data-ttu-id="07ac3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="07ac3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07ac3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="07ac3-120">Authorization</span></span>  | <span data-ttu-id="07ac3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07ac3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07ac3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="07ac3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="07ac3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="07ac3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07ac3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07ac3-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="07ac3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="07ac3-127">Response</span></span>

<span data-ttu-id="07ac3-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07ac3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07ac3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07ac3-130">Example</span></span>
<span data-ttu-id="07ac3-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="07ac3-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="07ac3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07ac3-132">Request</span></span>
<span data-ttu-id="07ac3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07ac3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="07ac3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07ac3-134">Response</span></span>
<span data-ttu-id="07ac3-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07ac3-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-refreshall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
