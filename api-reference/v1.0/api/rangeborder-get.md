---
title: Obter RangeBorder
description: Recupere as propriedades e os relacionamentos do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9495191b31b5451b876f0ae9f499ba2f5f1f44ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525534"
---
# <a name="get-rangeborder"></a><span data-ttu-id="13056-103">Obter RangeBorder</span><span class="sxs-lookup"><span data-stu-id="13056-103">Get RangeBorder</span></span>

<span data-ttu-id="13056-104">Recupere as propriedades e os relacionamentos do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="13056-104">Retrieve the properties and relationships of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="13056-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="13056-105">Permissions</span></span>
<span data-ttu-id="13056-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13056-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13056-108">Permission type</span></span>      | <span data-ttu-id="13056-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13056-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13056-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13056-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13056-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13056-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13056-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13056-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13056-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13056-113">Not supported.</span></span>    |
|<span data-ttu-id="13056-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13056-114">Application</span></span> | <span data-ttu-id="13056-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13056-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13056-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13056-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders/{sideIndex}
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13056-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13056-117">Optional query parameters</span></span>
<span data-ttu-id="13056-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13056-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13056-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13056-119">Request headers</span></span>
| <span data-ttu-id="13056-120">Nome</span><span class="sxs-lookup"><span data-stu-id="13056-120">Name</span></span>      |<span data-ttu-id="13056-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="13056-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13056-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13056-122">Authorization</span></span>  | <span data-ttu-id="13056-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13056-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13056-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="13056-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="13056-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="13056-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13056-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13056-128">Request body</span></span>
<span data-ttu-id="13056-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13056-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13056-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="13056-130">Response</span></span>

<span data-ttu-id="13056-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [WorkbookRangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13056-131">If successful, this method returns a `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13056-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13056-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13056-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13056-133">Request</span></span>
<span data-ttu-id="13056-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13056-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeborder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
```
##### <a name="response"></a><span data-ttu-id="13056-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="13056-135">Response</span></span>
<span data-ttu-id="13056-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13056-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
