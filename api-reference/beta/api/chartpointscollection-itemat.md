---
title: 'ChartPointsCollection: ItemAt'
description: Recupera um ponto com base na respectiva posição dentro da série.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 73bef5b16cd3748f0f7fc689a43653ceb9388ebb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439083"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="5c51c-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5c51c-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="5c51c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c51c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c51c-105">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="5c51c-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c51c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c51c-106">Permissions</span></span>
<span data-ttu-id="5c51c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c51c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c51c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c51c-109">Permission type</span></span>      | <span data-ttu-id="5c51c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c51c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c51c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c51c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c51c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c51c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c51c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c51c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c51c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c51c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c51c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c51c-115">Application</span></span> | <span data-ttu-id="5c51c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c51c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c51c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c51c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="5c51c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c51c-118">Request headers</span></span>
| <span data-ttu-id="5c51c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c51c-119">Name</span></span>       | <span data-ttu-id="5c51c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c51c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c51c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c51c-121">Authorization</span></span>  | <span data-ttu-id="5c51c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c51c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c51c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5c51c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c51c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c51c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c51c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c51c-127">Request body</span></span>
<span data-ttu-id="5c51c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c51c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c51c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c51c-129">Parameter</span></span>    | <span data-ttu-id="5c51c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c51c-130">Type</span></span>   |<span data-ttu-id="5c51c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c51c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c51c-132">index</span><span class="sxs-lookup"><span data-stu-id="5c51c-132">index</span></span>|<span data-ttu-id="5c51c-133">number</span><span class="sxs-lookup"><span data-stu-id="5c51c-133">number</span></span>|<span data-ttu-id="5c51c-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="5c51c-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5c51c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c51c-136">Response</span></span>

<span data-ttu-id="5c51c-137">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [workbookChartPoint](../resources/workbookchartpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c51c-137">If successful, this method returns `200 OK` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c51c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c51c-138">Example</span></span>
<span data-ttu-id="5c51c-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5c51c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c51c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c51c-140">Request</span></span>
<span data-ttu-id="5c51c-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c51c-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c51c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c51c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="5c51c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c51c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c51c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c51c-144">Response</span></span>
<span data-ttu-id="5c51c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c51c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
