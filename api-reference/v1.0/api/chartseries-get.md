---
title: Obter ChartSeries
description: Recupera as propriedades e os relacionamentos do objeto chartseries.
author: lumine2008
ms.openlocfilehash: ea89b115b2f812d4f0aaeb786096e766d97a5b1d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358174"
---
# <a name="get-chartseries"></a><span data-ttu-id="05b57-103">Obter ChartSeries</span><span class="sxs-lookup"><span data-stu-id="05b57-103">Get ChartSeries</span></span>

<span data-ttu-id="05b57-104">Recupera as propriedades e os relacionamentos do objeto chartseries.</span><span class="sxs-lookup"><span data-stu-id="05b57-104">Retrieve the properties and relationships of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="05b57-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="05b57-105">Permissions</span></span>
<span data-ttu-id="05b57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05b57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05b57-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05b57-108">Permission type</span></span>      | <span data-ttu-id="05b57-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05b57-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05b57-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05b57-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05b57-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05b57-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="05b57-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05b57-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05b57-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05b57-113">Not supported.</span></span>    |
|<span data-ttu-id="05b57-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05b57-114">Application</span></span> | <span data-ttu-id="05b57-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05b57-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05b57-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05b57-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05b57-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05b57-117">Optional query parameters</span></span>
<span data-ttu-id="05b57-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05b57-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05b57-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05b57-119">Request headers</span></span>
| <span data-ttu-id="05b57-120">Nome</span><span class="sxs-lookup"><span data-stu-id="05b57-120">Name</span></span>      |<span data-ttu-id="05b57-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="05b57-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05b57-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05b57-122">Authorization</span></span>  | <span data-ttu-id="05b57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05b57-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05b57-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="05b57-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="05b57-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="05b57-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05b57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05b57-128">Request body</span></span>
<span data-ttu-id="05b57-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05b57-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05b57-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="05b57-130">Response</span></span>

<span data-ttu-id="05b57-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [WorkbookChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05b57-131">If successful, this method returns a `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05b57-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05b57-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05b57-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05b57-133">Request</span></span>
<span data-ttu-id="05b57-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05b57-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartseries"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
##### <a name="response"></a><span data-ttu-id="05b57-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="05b57-135">Response</span></span>
<span data-ttu-id="05b57-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05b57-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->