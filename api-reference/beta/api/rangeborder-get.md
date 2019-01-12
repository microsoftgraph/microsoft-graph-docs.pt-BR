---
title: Obter RangeBorder
description: Recupere as propriedades e os relacionamentos do objeto rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7803d80a192f1b58adbd7e658cf61f4bace4dbdb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931269"
---
# <a name="get-rangeborder"></a><span data-ttu-id="f184d-103">Obter RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f184d-103">Get RangeBorder</span></span>

> <span data-ttu-id="f184d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f184d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f184d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f184d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f184d-106">Recupere as propriedades e os relacionamentos do objeto rangeborder.</span><span class="sxs-lookup"><span data-stu-id="f184d-106">Retrieve the properties and relationships of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f184d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f184d-107">Permissions</span></span>
<span data-ttu-id="f184d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f184d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f184d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f184d-110">Permission type</span></span>      | <span data-ttu-id="f184d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f184d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f184d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f184d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f184d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f184d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f184d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f184d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f184d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f184d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f184d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f184d-116">Application</span></span> | <span data-ttu-id="f184d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f184d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f184d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f184d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/borders(<sideIndex>)
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f184d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f184d-119">Optional query parameters</span></span>
<span data-ttu-id="f184d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f184d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f184d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f184d-121">Request headers</span></span>
| <span data-ttu-id="f184d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f184d-122">Name</span></span>      |<span data-ttu-id="f184d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f184d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f184d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f184d-124">Authorization</span></span>  | <span data-ttu-id="f184d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f184d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f184d-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f184d-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="f184d-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f184d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f184d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f184d-130">Request body</span></span>
<span data-ttu-id="f184d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f184d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f184d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f184d-132">Response</span></span>

<span data-ttu-id="f184d-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [RangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f184d-133">If successful, this method returns a `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f184d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f184d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f184d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f184d-135">Request</span></span>
<span data-ttu-id="f184d-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f184d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeborder"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
```
##### <a name="response"></a><span data-ttu-id="f184d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f184d-137">Response</span></span>
<span data-ttu-id="f184d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f184d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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
