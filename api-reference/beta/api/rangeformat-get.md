---
title: Obter RangeFormat
description: Recupere as propriedades e os relacionamentos do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fd6b1db175e5efe0e349ac5c1f0e07b2da243b27
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336779"
---
# <a name="get-rangeformat"></a><span data-ttu-id="bdf19-103">Obter RangeFormat</span><span class="sxs-lookup"><span data-stu-id="bdf19-103">Get RangeFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf19-104">Recupere as propriedades e os relacionamentos do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="bdf19-104">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bdf19-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdf19-105">Permissions</span></span>
<span data-ttu-id="bdf19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf19-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdf19-108">Permission type</span></span>      | <span data-ttu-id="bdf19-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdf19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdf19-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdf19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdf19-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdf19-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdf19-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdf19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf19-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdf19-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdf19-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdf19-114">Application</span></span> | <span data-ttu-id="bdf19-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdf19-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdf19-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bdf19-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bdf19-117">Optional query parameters</span></span>
<span data-ttu-id="bdf19-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf19-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdf19-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf19-119">Request headers</span></span>
| <span data-ttu-id="bdf19-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bdf19-120">Name</span></span>      |<span data-ttu-id="bdf19-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf19-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bdf19-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdf19-122">Authorization</span></span>  | <span data-ttu-id="bdf19-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdf19-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdf19-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bdf19-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bdf19-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bdf19-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdf19-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf19-128">Request body</span></span>
<span data-ttu-id="bdf19-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bdf19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf19-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf19-130">Response</span></span>

<span data-ttu-id="bdf19-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookRangeFormat](../resources/workbookrangeformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf19-131">If successful, this method returns a `200 OK` response code and [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdf19-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdf19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdf19-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf19-133">Request</span></span>
<span data-ttu-id="bdf19-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdf19-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format
```
##### <a name="response"></a><span data-ttu-id="bdf19-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf19-135">Response</span></span>
<span data-ttu-id="bdf19-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdf19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
