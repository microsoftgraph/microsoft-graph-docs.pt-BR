---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f91b5044c470430d8d508cab3585db48b51048bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995864"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="03838-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="03838-104">workbookRange: visibleView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="03838-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="03838-105">Permissions</span></span>
<span data-ttu-id="03838-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03838-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03838-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03838-108">Permission type</span></span>      | <span data-ttu-id="03838-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03838-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03838-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03838-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03838-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03838-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03838-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03838-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03838-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03838-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03838-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03838-114">Application</span></span> | <span data-ttu-id="03838-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03838-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03838-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03838-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="03838-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03838-117">Request headers</span></span>
| <span data-ttu-id="03838-118">Nome</span><span class="sxs-lookup"><span data-stu-id="03838-118">Name</span></span>       | <span data-ttu-id="03838-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="03838-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03838-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="03838-120">Authorization</span></span>  | <span data-ttu-id="03838-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03838-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03838-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03838-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="03838-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="03838-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03838-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03838-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="03838-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="03838-127">Response</span></span>

<span data-ttu-id="03838-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03838-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03838-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03838-129">Example</span></span>
<span data-ttu-id="03838-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="03838-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03838-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03838-131">Request</span></span>
<span data-ttu-id="03838-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03838-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="03838-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="03838-133">Response</span></span>
<span data-ttu-id="03838-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03838-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
