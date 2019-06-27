---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos do objeto workbookApplication.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a7b175ae9c9446f3e2938a75aab88eaadc642d9c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269437"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="9824d-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="9824d-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9824d-104">Recupere as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="9824d-104">Retrieve the properties and relationships of workbookApplication object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9824d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9824d-105">Permissions</span></span>
<span data-ttu-id="9824d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9824d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9824d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9824d-108">Permission type</span></span>      | <span data-ttu-id="9824d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9824d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9824d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9824d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9824d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9824d-111">Not supported.</span></span>    |
|<span data-ttu-id="9824d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9824d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9824d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9824d-113">Not supported.</span></span>    |
|<span data-ttu-id="9824d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9824d-114">Application</span></span> | <span data-ttu-id="9824d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9824d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9824d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9824d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9824d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9824d-117">Optional query parameters</span></span>
<span data-ttu-id="9824d-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9824d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9824d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9824d-119">Request headers</span></span>
| <span data-ttu-id="9824d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9824d-120">Name</span></span>      |<span data-ttu-id="9824d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9824d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9824d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9824d-122">Authorization</span></span>  | <span data-ttu-id="9824d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9824d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9824d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9824d-125">Request body</span></span>
<span data-ttu-id="9824d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9824d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9824d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9824d-127">Response</span></span>

<span data-ttu-id="9824d-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9824d-128">If successful, this method returns a `200 OK` response code and [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9824d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9824d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9824d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9824d-130">Request</span></span>
<span data-ttu-id="9824d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9824d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="9824d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9824d-132">Response</span></span>
<span data-ttu-id="9824d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9824d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9824d-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9824d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9824d-137">C#</span><span class="sxs-lookup"><span data-stu-id="9824d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_workbookApplication-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9824d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9824d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_workbookApplication-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9824d-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9824d-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_workbookApplication-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookapplication-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookapplication-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
