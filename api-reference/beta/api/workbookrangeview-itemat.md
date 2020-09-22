---
title: 'workbookRangeView: itemAt'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 02e46192fa77009a25e9f8fe8158e544c970baeb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022033"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="6df22-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="6df22-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="6df22-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6df22-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="6df22-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6df22-106">Permissions</span></span>
<span data-ttu-id="6df22-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6df22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6df22-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6df22-109">Permission type</span></span>      | <span data-ttu-id="6df22-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6df22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6df22-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6df22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6df22-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6df22-112">Not supported.</span></span>    |
|<span data-ttu-id="6df22-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6df22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6df22-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6df22-114">Not supported.</span></span>    |
|<span data-ttu-id="6df22-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6df22-115">Application</span></span> | <span data-ttu-id="6df22-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6df22-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6df22-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6df22-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="6df22-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6df22-118">Request headers</span></span>
| <span data-ttu-id="6df22-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6df22-119">Name</span></span>       | <span data-ttu-id="6df22-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6df22-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6df22-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6df22-121">Authorization</span></span>  | <span data-ttu-id="6df22-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6df22-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6df22-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6df22-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6df22-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6df22-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6df22-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6df22-127">Request body</span></span>
<span data-ttu-id="6df22-128">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="6df22-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="6df22-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6df22-129">Parameter</span></span>    | <span data-ttu-id="6df22-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6df22-130">Type</span></span>   |<span data-ttu-id="6df22-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6df22-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6df22-132">índice</span><span class="sxs-lookup"><span data-stu-id="6df22-132">index</span></span>|<span data-ttu-id="6df22-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6df22-133">Int32</span></span>|<span data-ttu-id="6df22-134">O índice do item a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="6df22-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="6df22-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6df22-135">Response</span></span>

<span data-ttu-id="6df22-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6df22-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6df22-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6df22-137">Example</span></span>
<span data-ttu-id="6df22-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6df22-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6df22-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6df22-139">Request</span></span>
<span data-ttu-id="6df22-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6df22-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="6df22-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6df22-141">Response</span></span>
<span data-ttu-id="6df22-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6df22-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


