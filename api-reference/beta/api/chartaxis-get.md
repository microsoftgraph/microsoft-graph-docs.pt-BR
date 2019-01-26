---
title: Obter ChartAxis
description: Lê as propriedades e os relacionamentos do objeto chartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9fd966aa8cfa0ebd39d586d36f952e144989072f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571706"
---
# <a name="get-chartaxis"></a><span data-ttu-id="467c4-103">Obter ChartAxis</span><span class="sxs-lookup"><span data-stu-id="467c4-103">Get ChartAxis</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="467c4-104">Lê as propriedades e os relacionamentos do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="467c4-104">Retrieve the properties and relationships of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="467c4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="467c4-105">Permissions</span></span>
<span data-ttu-id="467c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="467c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="467c4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="467c4-108">Permission type</span></span>      | <span data-ttu-id="467c4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="467c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="467c4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="467c4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="467c4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="467c4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="467c4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="467c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="467c4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="467c4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="467c4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="467c4-114">Application</span></span> | <span data-ttu-id="467c4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="467c4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="467c4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="467c4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-query-parameters"></a><span data-ttu-id="467c4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="467c4-117">Optional query parameters</span></span>
<span data-ttu-id="467c4-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="467c4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="467c4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="467c4-119">Request headers</span></span>
| <span data-ttu-id="467c4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="467c4-120">Name</span></span>      |<span data-ttu-id="467c4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="467c4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="467c4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="467c4-122">Authorization</span></span>  | <span data-ttu-id="467c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="467c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="467c4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="467c4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="467c4-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="467c4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="467c4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="467c4-128">Request body</span></span>
<span data-ttu-id="467c4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="467c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="467c4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="467c4-130">Response</span></span>

<span data-ttu-id="467c4-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxis](../resources/chartaxis.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="467c4-131">If successful, this method returns a `200 OK` response code and [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="467c4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="467c4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="467c4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="467c4-133">Request</span></span>
<span data-ttu-id="467c4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="467c4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartaxis"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
```
##### <a name="response"></a><span data-ttu-id="467c4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="467c4-135">Response</span></span>
<span data-ttu-id="467c4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="467c4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartAxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxis-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
