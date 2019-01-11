---
title: 'workbookRangeView: itemAt'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
ms.openlocfilehash: 2fc5c638bbe55f3209d629415023ece7d81e6c29
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834773"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="82ebd-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="82ebd-104">workbookRangeView: itemAt</span></span>

> <span data-ttu-id="82ebd-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82ebd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82ebd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82ebd-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="82ebd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="82ebd-107">Permissions</span></span>
<span data-ttu-id="82ebd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82ebd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82ebd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82ebd-110">Permission type</span></span>      | <span data-ttu-id="82ebd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82ebd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82ebd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82ebd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82ebd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82ebd-113">Not supported.</span></span>    |
|<span data-ttu-id="82ebd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82ebd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82ebd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82ebd-115">Not supported.</span></span>    |
|<span data-ttu-id="82ebd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82ebd-116">Application</span></span> | <span data-ttu-id="82ebd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82ebd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82ebd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82ebd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="82ebd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82ebd-119">Request headers</span></span>
| <span data-ttu-id="82ebd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="82ebd-120">Name</span></span>       | <span data-ttu-id="82ebd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ebd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="82ebd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="82ebd-122">Authorization</span></span>  | <span data-ttu-id="82ebd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82ebd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82ebd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="82ebd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="82ebd-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="82ebd-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82ebd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82ebd-128">Request body</span></span>
<span data-ttu-id="82ebd-129">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="82ebd-129">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="82ebd-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="82ebd-130">Parameter</span></span>    | <span data-ttu-id="82ebd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82ebd-131">Type</span></span>   |<span data-ttu-id="82ebd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ebd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82ebd-133">índice</span><span class="sxs-lookup"><span data-stu-id="82ebd-133">index</span></span>|<span data-ttu-id="82ebd-134">Int32</span><span class="sxs-lookup"><span data-stu-id="82ebd-134">Int32</span></span>|<span data-ttu-id="82ebd-135">O índice do item a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="82ebd-135">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="82ebd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="82ebd-136">Response</span></span>

<span data-ttu-id="82ebd-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82ebd-137">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82ebd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82ebd-138">Example</span></span>
<span data-ttu-id="82ebd-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="82ebd-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="82ebd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82ebd-140">Request</span></span>
<span data-ttu-id="82ebd-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82ebd-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="82ebd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="82ebd-142">Response</span></span>
<span data-ttu-id="82ebd-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82ebd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
