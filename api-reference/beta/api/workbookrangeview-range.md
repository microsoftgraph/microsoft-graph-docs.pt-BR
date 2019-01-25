---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b6a1b678b77cf4bd4d20d9d3d0a68178dbc07151
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526918"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="83b7e-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="83b7e-103">workbookRangeView: range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83b7e-104">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="83b7e-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="83b7e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="83b7e-105">Permissions</span></span>
<span data-ttu-id="83b7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83b7e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83b7e-108">Permission type</span></span>      | <span data-ttu-id="83b7e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83b7e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83b7e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83b7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83b7e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83b7e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83b7e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83b7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83b7e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83b7e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83b7e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83b7e-114">Application</span></span> | <span data-ttu-id="83b7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83b7e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83b7e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83b7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="83b7e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83b7e-117">Request headers</span></span>
| <span data-ttu-id="83b7e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="83b7e-118">Name</span></span>       | <span data-ttu-id="83b7e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="83b7e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83b7e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="83b7e-120">Authorization</span></span>  | <span data-ttu-id="83b7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83b7e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83b7e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="83b7e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="83b7e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="83b7e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83b7e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83b7e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="83b7e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b7e-127">Response</span></span>

<span data-ttu-id="83b7e-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83b7e-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b7e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83b7e-129">Example</span></span>
<span data-ttu-id="83b7e-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="83b7e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="83b7e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83b7e-131">Request</span></span>
<span data-ttu-id="83b7e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83b7e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="83b7e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b7e-133">Response</span></span>
<span data-ttu-id="83b7e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83b7e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
