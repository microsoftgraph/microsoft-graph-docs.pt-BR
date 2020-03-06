---
title: 'workbookRangeView: itemAt'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 35ca224c5e46359672ee48e2e62b6a0b56a68377
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508720"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="1dd0b-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="1dd0b-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="1dd0b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd0b-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="1dd0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dd0b-106">Permissions</span></span>
<span data-ttu-id="1dd0b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dd0b-109">Permission type</span></span>      | <span data-ttu-id="1dd0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dd0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dd0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1dd0b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dd0b-112">Files.ReadWrite</span></span> |
|<span data-ttu-id="1dd0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dd0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-114">Not supported.</span></span>    |
|<span data-ttu-id="1dd0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dd0b-115">Application</span></span> | <span data-ttu-id="1dd0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd0b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="1dd0b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd0b-118">Request headers</span></span>
| <span data-ttu-id="1dd0b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1dd0b-119">Name</span></span>       | <span data-ttu-id="1dd0b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd0b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1dd0b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dd0b-121">Authorization</span></span>  | <span data-ttu-id="1dd0b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dd0b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1dd0b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1dd0b-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="1dd0b-127">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1dd0b-127">Function parameters</span></span>
<span data-ttu-id="1dd0b-128">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="1dd0b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1dd0b-129">Parameter</span></span>    | <span data-ttu-id="1dd0b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dd0b-130">Type</span></span>   |<span data-ttu-id="1dd0b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd0b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dd0b-132">índice</span><span class="sxs-lookup"><span data-stu-id="1dd0b-132">index</span></span>|<span data-ttu-id="1dd0b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1dd0b-133">Int32</span></span>|<span data-ttu-id="1dd0b-134">O índice do item a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="1dd0b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd0b-135">Response</span></span>

<span data-ttu-id="1dd0b-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd0b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dd0b-137">Example</span></span>
<span data-ttu-id="1dd0b-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1dd0b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd0b-139">Request</span></span>
<span data-ttu-id="1dd0b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="1dd0b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd0b-141">Response</span></span>
<span data-ttu-id="1dd0b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dd0b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
