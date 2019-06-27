---
title: Obter NamedItem
description: Recupere as propriedades e os relacionamentos do objeto nameditem.
localization_priority: Normal
ms.openlocfilehash: b05dbdf6681431604d14d4f22921a57fc793e5ed
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268611"
---
# <a name="get-nameditem"></a><span data-ttu-id="dfed6-103">Obter NamedItem</span><span class="sxs-lookup"><span data-stu-id="dfed6-103">Get NamedItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfed6-104">Recupere as propriedades e os relacionamentos do objeto nameditem.</span><span class="sxs-lookup"><span data-stu-id="dfed6-104">Retrieve the properties and relationships of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfed6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfed6-105">Permissions</span></span>
<span data-ttu-id="dfed6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfed6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfed6-108">Permission type</span></span>      | <span data-ttu-id="dfed6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfed6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfed6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfed6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfed6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfed6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfed6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfed6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfed6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfed6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfed6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfed6-114">Application</span></span> | <span data-ttu-id="dfed6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfed6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfed6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfed6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfed6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfed6-117">Optional query parameters</span></span>
<span data-ttu-id="dfed6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfed6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfed6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfed6-119">Request headers</span></span>
| <span data-ttu-id="dfed6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dfed6-120">Name</span></span>      |<span data-ttu-id="dfed6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfed6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfed6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfed6-122">Authorization</span></span>  | <span data-ttu-id="dfed6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfed6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfed6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dfed6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dfed6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dfed6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfed6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfed6-128">Request body</span></span>
<span data-ttu-id="dfed6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfed6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfed6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfed6-130">Response</span></span>

<span data-ttu-id="dfed6-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookNamedItem](../resources/workbooknameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfed6-131">If successful, this method returns a `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfed6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfed6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfed6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfed6-133">Request</span></span>
<span data-ttu-id="dfed6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfed6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_nameditem"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}
```
##### <a name="response"></a><span data-ttu-id="dfed6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfed6-135">Response</span></span>
<span data-ttu-id="dfed6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfed6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed6-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dfed6-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed6-140">C#</span><span class="sxs-lookup"><span data-stu-id="dfed6-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_nameditem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed6-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed6-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_nameditem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed6-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dfed6-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_nameditem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get NamedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/nameditem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/nameditem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
