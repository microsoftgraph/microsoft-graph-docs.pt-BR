---
title: Obter RangeFormat
description: Recupere as propriedades e os relacionamentos do objeto rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ee0d6e46dc59d70256f182da35cfd4254c9c3ea9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936517"
---
# <a name="get-rangeformat"></a><span data-ttu-id="1c2c8-103">Obter RangeFormat</span><span class="sxs-lookup"><span data-stu-id="1c2c8-103">Get RangeFormat</span></span>

> <span data-ttu-id="1c2c8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c2c8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c2c8-106">Recupere as propriedades e os relacionamentos do objeto rangeformat.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-106">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c2c8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c2c8-107">Permissions</span></span>
<span data-ttu-id="1c2c8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c2c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c2c8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c2c8-110">Permission type</span></span>      | <span data-ttu-id="1c2c8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c2c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c2c8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c2c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1c2c8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c2c8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c2c8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c2c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c2c8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c2c8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c2c8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c2c8-116">Application</span></span> | <span data-ttu-id="1c2c8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c2c8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c2c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c2c8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c2c8-119">Optional query parameters</span></span>
<span data-ttu-id="1c2c8-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c2c8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c2c8-121">Request headers</span></span>
| <span data-ttu-id="1c2c8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1c2c8-122">Name</span></span>      |<span data-ttu-id="1c2c8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c2c8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c2c8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c2c8-124">Authorization</span></span>  | <span data-ttu-id="1c2c8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c2c8-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c2c8-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c2c8-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c2c8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c2c8-130">Request body</span></span>
<span data-ttu-id="1c2c8-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c2c8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c2c8-132">Response</span></span>

<span data-ttu-id="1c2c8-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFormat](../resources/rangeformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-133">If successful, this method returns a `200 OK` response code and [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c2c8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c2c8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c2c8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c2c8-135">Request</span></span>
<span data-ttu-id="1c2c8-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format
```
##### <a name="response"></a><span data-ttu-id="1c2c8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c2c8-137">Response</span></span>
<span data-ttu-id="1c2c8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c2c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
