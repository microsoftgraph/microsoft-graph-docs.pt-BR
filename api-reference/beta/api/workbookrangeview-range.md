---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 16a9ffabf5462b15186cbd21f9f243419cad1e3f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996120"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="5efac-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="5efac-103">workbookRangeView: range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5efac-104">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="5efac-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="5efac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5efac-105">Permissions</span></span>
<span data-ttu-id="5efac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5efac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5efac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5efac-108">Permission type</span></span>      | <span data-ttu-id="5efac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5efac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5efac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5efac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5efac-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5efac-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5efac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5efac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5efac-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5efac-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5efac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5efac-114">Application</span></span> | <span data-ttu-id="5efac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5efac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5efac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5efac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="5efac-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5efac-117">Request headers</span></span>
| <span data-ttu-id="5efac-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5efac-118">Name</span></span>       | <span data-ttu-id="5efac-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efac-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5efac-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5efac-120">Authorization</span></span>  | <span data-ttu-id="5efac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5efac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5efac-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5efac-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5efac-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5efac-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5efac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5efac-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5efac-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5efac-127">Response</span></span>

<span data-ttu-id="5efac-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5efac-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5efac-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5efac-129">Example</span></span>
<span data-ttu-id="5efac-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5efac-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5efac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5efac-131">Request</span></span>
<span data-ttu-id="5efac-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5efac-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5efac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5efac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5efac-134">C#</span><span class="sxs-lookup"><span data-stu-id="5efac-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5efac-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5efac-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5efac-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5efac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5efac-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5efac-137">Response</span></span>
<span data-ttu-id="5efac-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5efac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
