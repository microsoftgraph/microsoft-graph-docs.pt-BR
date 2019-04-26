---
title: Obter workbookChartAxisTitle
description: Recupere as propriedades e os relacionamentos do objeto workbookchartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1d953c41d64d0b9afae3fb090185cea7620fc8e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327812"
---
# <a name="get-workbookchartaxistitle"></a><span data-ttu-id="71ee3-103">Obter workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="71ee3-103">Get workbookChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71ee3-104">Recupera as propriedades e os relacionamentos do objeto chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="71ee3-104">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71ee3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="71ee3-105">Permissions</span></span>
<span data-ttu-id="71ee3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ee3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ee3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71ee3-108">Permission type</span></span>      | <span data-ttu-id="71ee3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71ee3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71ee3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71ee3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71ee3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71ee3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71ee3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71ee3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71ee3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71ee3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71ee3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71ee3-114">Application</span></span> | <span data-ttu-id="71ee3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ee3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71ee3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71ee3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71ee3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71ee3-117">Optional query parameters</span></span>
<span data-ttu-id="71ee3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71ee3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71ee3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71ee3-119">Request headers</span></span>
| <span data-ttu-id="71ee3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="71ee3-120">Name</span></span>      |<span data-ttu-id="71ee3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ee3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71ee3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71ee3-122">Authorization</span></span>  | <span data-ttu-id="71ee3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71ee3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71ee3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71ee3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71ee3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="71ee3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ee3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71ee3-128">Request body</span></span>
<span data-ttu-id="71ee3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71ee3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71ee3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ee3-130">Response</span></span>

<span data-ttu-id="71ee3-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71ee3-131">If successful, this method returns a `200 OK` response code and [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71ee3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71ee3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71ee3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71ee3-133">Request</span></span>
<span data-ttu-id="71ee3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71ee3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
```
##### <a name="response"></a><span data-ttu-id="71ee3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ee3-135">Response</span></span>
<span data-ttu-id="71ee3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71ee3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
