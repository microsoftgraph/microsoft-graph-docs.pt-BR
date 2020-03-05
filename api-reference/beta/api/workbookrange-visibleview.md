---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1ad82583c8cb574138c901c733211728bfc225bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451333"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="da5fb-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="da5fb-104">workbookRange: visibleView</span></span>

<span data-ttu-id="da5fb-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da5fb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="da5fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da5fb-106">Permissions</span></span>
<span data-ttu-id="da5fb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da5fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da5fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da5fb-109">Permission type</span></span>      | <span data-ttu-id="da5fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da5fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da5fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da5fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da5fb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da5fb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da5fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da5fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da5fb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da5fb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da5fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da5fb-115">Application</span></span> | <span data-ttu-id="da5fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da5fb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da5fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da5fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="da5fb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da5fb-118">Request headers</span></span>
| <span data-ttu-id="da5fb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="da5fb-119">Name</span></span>       | <span data-ttu-id="da5fb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da5fb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da5fb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da5fb-121">Authorization</span></span>  | <span data-ttu-id="da5fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da5fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da5fb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da5fb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="da5fb-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="da5fb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da5fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da5fb-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="da5fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="da5fb-128">Response</span></span>

<span data-ttu-id="da5fb-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da5fb-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da5fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da5fb-130">Example</span></span>
<span data-ttu-id="da5fb-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="da5fb-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da5fb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da5fb-132">Request</span></span>
<span data-ttu-id="da5fb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da5fb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da5fb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="da5fb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="da5fb-135">C#</span><span class="sxs-lookup"><span data-stu-id="da5fb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da5fb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da5fb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da5fb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da5fb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da5fb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="da5fb-138">Response</span></span>
<span data-ttu-id="da5fb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da5fb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
