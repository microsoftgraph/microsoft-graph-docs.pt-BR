---
title: Obter intervalo
description: Recupere as propriedades e os relacionamentos do objeto de intervalo.
author: lumine2008
ms.openlocfilehash: 3914f018da434536dca280fac2536e93e5496ea9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347247"
---
# <a name="get-range"></a><span data-ttu-id="cac21-103">Obter intervalo</span><span class="sxs-lookup"><span data-stu-id="cac21-103">Get Range</span></span>

<span data-ttu-id="cac21-104">Recupere as propriedades e os relacionamentos do objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="cac21-104">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cac21-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cac21-105">Permissions</span></span>
<span data-ttu-id="cac21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cac21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac21-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cac21-108">Permission type</span></span>      | <span data-ttu-id="cac21-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cac21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cac21-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cac21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cac21-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cac21-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cac21-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cac21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cac21-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cac21-113">Not supported.</span></span>    |
|<span data-ttu-id="cac21-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cac21-114">Application</span></span> | <span data-ttu-id="cac21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cac21-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cac21-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cac21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range(address='<address>')
GET /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cac21-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cac21-117">Optional query parameters</span></span>
<span data-ttu-id="cac21-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cac21-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cac21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cac21-119">Request headers</span></span>
| <span data-ttu-id="cac21-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cac21-120">Name</span></span>      |<span data-ttu-id="cac21-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cac21-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cac21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cac21-122">Authorization</span></span>  | <span data-ttu-id="cac21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cac21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cac21-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cac21-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cac21-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="cac21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac21-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cac21-128">Request body</span></span>
<span data-ttu-id="cac21-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cac21-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cac21-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cac21-130">Response</span></span>

<span data-ttu-id="cac21-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cac21-131">If successful, this method returns a `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cac21-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cac21-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cac21-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cac21-133">Request</span></span>
<span data-ttu-id="cac21-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cac21-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
##### <a name="response"></a><span data-ttu-id="cac21-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cac21-135">Response</span></span>
<span data-ttu-id="cac21-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cac21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->