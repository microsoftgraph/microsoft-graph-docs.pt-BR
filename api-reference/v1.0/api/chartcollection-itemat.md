---
title: 'ChartCollection: ItemAt'
description: Obtém um gráfico com base em sua posição na coleção.
ms.openlocfilehash: dd685859be6b179e074d65e952b5dbda4bdbc7d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006570"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="8c827-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="8c827-103">ChartCollection: ItemAt</span></span>

<span data-ttu-id="8c827-104">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="8c827-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c827-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c827-105">Permissions</span></span>
<span data-ttu-id="8c827-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c827-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c827-108">Permission type</span></span>      | <span data-ttu-id="8c827-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c827-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c827-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c827-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c827-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c827-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c827-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c827-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c827-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c827-113">Not supported.</span></span>    |
|<span data-ttu-id="8c827-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c827-114">Application</span></span> | <span data-ttu-id="8c827-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c827-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c827-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c827-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="8c827-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c827-117">Request headers</span></span>
| <span data-ttu-id="8c827-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8c827-118">Name</span></span>       | <span data-ttu-id="8c827-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c827-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c827-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c827-120">Authorization</span></span>  | <span data-ttu-id="8c827-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c827-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c827-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8c827-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c827-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8c827-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c827-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c827-126">Request body</span></span>
<span data-ttu-id="8c827-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c827-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c827-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8c827-128">Parameter</span></span>    | <span data-ttu-id="8c827-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c827-129">Type</span></span>   |<span data-ttu-id="8c827-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c827-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c827-131">índice</span><span class="sxs-lookup"><span data-stu-id="8c827-131">index</span></span>|<span data-ttu-id="8c827-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8c827-132">Int32</span></span>|<span data-ttu-id="8c827-p104">Valor de índice do objeto a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="8c827-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="8c827-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c827-135">Response</span></span>

<span data-ttu-id="8c827-136">Se tiver êxito, este método retornará `200 OK` código de resposta e o objeto [WorkbookChart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c827-136">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c827-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c827-137">Example</span></span>
<span data-ttu-id="8c827-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8c827-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c827-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c827-139">Request</span></span>
<span data-ttu-id="8c827-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c827-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```

##### <a name="response"></a><span data-ttu-id="8c827-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c827-141">Response</span></span>
<span data-ttu-id="8c827-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c827-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->