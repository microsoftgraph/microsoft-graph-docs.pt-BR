---
title: Criar ChartSeries
description: Use essa API para criar novas ChartSeries.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a86ccc050d9cde4cc8f7fc37222b3401bbb0d768
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859805"
---
# <a name="create-chartseries"></a><span data-ttu-id="9a1fd-103">Criar ChartSeries</span><span class="sxs-lookup"><span data-stu-id="9a1fd-103">Create ChartSeries</span></span>

> <span data-ttu-id="9a1fd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a1fd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a1fd-106">Use essa API para criar novas ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-106">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a1fd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a1fd-107">Permissions</span></span>
<span data-ttu-id="9a1fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a1fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a1fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a1fd-110">Permission type</span></span>      | <span data-ttu-id="9a1fd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a1fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a1fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a1fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a1fd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a1fd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a1fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a1fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a1fd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a1fd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a1fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a1fd-116">Application</span></span> | <span data-ttu-id="9a1fd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a1fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a1fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="9a1fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a1fd-119">Request headers</span></span>
| <span data-ttu-id="9a1fd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9a1fd-120">Name</span></span>       | <span data-ttu-id="9a1fd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a1fd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a1fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a1fd-122">Authorization</span></span>  | <span data-ttu-id="9a1fd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a1fd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a1fd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a1fd-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a1fd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a1fd-128">Request body</span></span>
<span data-ttu-id="9a1fd-129">No corpo da solicitação, forneça uma representação JSON do objeto [ChartSeries](../resources/chartseries.md).</span><span class="sxs-lookup"><span data-stu-id="9a1fd-129">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9a1fd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a1fd-130">Response</span></span>

<span data-ttu-id="9a1fd-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ChartSeries](../resources/chartseries.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-131">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a1fd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a1fd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a1fd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a1fd-133">Request</span></span>
<span data-ttu-id="9a1fd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="9a1fd-135">No corpo da solicitação, forneça uma representação JSON do objeto [ChartSeries](../resources/chartseries.md).</span><span class="sxs-lookup"><span data-stu-id="9a1fd-135">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9a1fd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a1fd-136">Response</span></span>
<span data-ttu-id="9a1fd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a1fd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
