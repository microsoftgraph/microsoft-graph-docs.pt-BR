---
title: Listar ChartCollection
description: Recupere uma lista de objetos de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f20ce9298ebf61b080a8d815e7b87579322b307b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640228"
---
# <a name="list-chartcollection"></a><span data-ttu-id="2990d-103">Listar ChartCollection</span><span class="sxs-lookup"><span data-stu-id="2990d-103">List ChartCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2990d-104">Recupere uma lista de objetos de gráfico.</span><span class="sxs-lookup"><span data-stu-id="2990d-104">Retrieve a list of chart objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2990d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2990d-105">Permissions</span></span>
<span data-ttu-id="2990d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2990d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2990d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2990d-108">Permission type</span></span>      | <span data-ttu-id="2990d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2990d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2990d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2990d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2990d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2990d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2990d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2990d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2990d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2990d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2990d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2990d-114">Application</span></span> | <span data-ttu-id="2990d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2990d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2990d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2990d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2990d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2990d-117">Optional query parameters</span></span>
<span data-ttu-id="2990d-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2990d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2990d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2990d-119">Request headers</span></span>
| <span data-ttu-id="2990d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2990d-120">Name</span></span>      |<span data-ttu-id="2990d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2990d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2990d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2990d-122">Authorization</span></span>  | <span data-ttu-id="2990d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2990d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2990d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2990d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2990d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2990d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2990d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2990d-128">Request body</span></span>
<span data-ttu-id="2990d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2990d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2990d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2990d-130">Response</span></span>

<span data-ttu-id="2990d-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Chart](../resources/chart.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2990d-131">If successful, this method returns a `200 OK` response code and collection of [Chart](../resources/chart.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2990d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2990d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2990d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2990d-133">Request</span></span>
<span data-ttu-id="2990d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2990d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartcollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
```
##### <a name="response"></a><span data-ttu-id="2990d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2990d-135">Response</span></span>
<span data-ttu-id="2990d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2990d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 93

{
  "value": [
    {
      "id": "id-value",
      "height": 99,
      "left": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ChartCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
