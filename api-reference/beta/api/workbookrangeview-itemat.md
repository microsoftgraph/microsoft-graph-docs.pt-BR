---
title: 'workbookRangeView: itemAt'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 85dcf4efd1cbbeae56b1f200ef53f48d19641369
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529898"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="8bcaf-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="8bcaf-104">workbookRangeView: itemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="8bcaf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bcaf-105">Permissions</span></span>
<span data-ttu-id="8bcaf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bcaf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bcaf-108">Permission type</span></span>      | <span data-ttu-id="8bcaf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bcaf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bcaf-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-111">Not supported.</span></span>    |
|<span data-ttu-id="8bcaf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bcaf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-113">Not supported.</span></span>    |
|<span data-ttu-id="8bcaf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bcaf-114">Application</span></span> | <span data-ttu-id="8bcaf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bcaf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bcaf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="8bcaf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcaf-117">Request headers</span></span>
| <span data-ttu-id="8bcaf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8bcaf-118">Name</span></span>       | <span data-ttu-id="8bcaf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bcaf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8bcaf-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bcaf-120">Authorization</span></span>  | <span data-ttu-id="8bcaf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bcaf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8bcaf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8bcaf-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bcaf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcaf-126">Request body</span></span>
<span data-ttu-id="8bcaf-127">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="8bcaf-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8bcaf-128">Parameter</span></span>    | <span data-ttu-id="8bcaf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bcaf-129">Type</span></span>   |<span data-ttu-id="8bcaf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bcaf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bcaf-131">índice</span><span class="sxs-lookup"><span data-stu-id="8bcaf-131">index</span></span>|<span data-ttu-id="8bcaf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8bcaf-132">Int32</span></span>|<span data-ttu-id="8bcaf-133">O índice do item a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="8bcaf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bcaf-134">Response</span></span>

<span data-ttu-id="8bcaf-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bcaf-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bcaf-136">Example</span></span>
<span data-ttu-id="8bcaf-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8bcaf-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bcaf-138">Request</span></span>
<span data-ttu-id="8bcaf-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="8bcaf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bcaf-140">Response</span></span>
<span data-ttu-id="8bcaf-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
