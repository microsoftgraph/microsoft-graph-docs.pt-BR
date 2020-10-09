---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e20cf77e307a1ea47212f8a40fd37ccbf5cfc07f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402776"
---
# <a name="get-icon"></a><span data-ttu-id="f5ee8-103">Get Icon</span><span class="sxs-lookup"><span data-stu-id="f5ee8-103">Get Icon</span></span>

<span data-ttu-id="f5ee8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ee8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5ee8-105">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5ee8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5ee8-106">Permissions</span></span>
<span data-ttu-id="f5ee8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ee8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5ee8-109">Permission type</span></span>      | <span data-ttu-id="f5ee8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5ee8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5ee8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5ee8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f5ee8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5ee8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5ee8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5ee8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ee8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-114">Not supported.</span></span>    |
|<span data-ttu-id="f5ee8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5ee8-115">Application</span></span> | <span data-ttu-id="f5ee8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5ee8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ee8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5ee8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5ee8-118">Optional query parameters</span></span>
<span data-ttu-id="f5ee8-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5ee8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ee8-120">Request headers</span></span>
| <span data-ttu-id="f5ee8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f5ee8-121">Name</span></span>      |<span data-ttu-id="f5ee8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ee8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5ee8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ee8-123">Authorization</span></span>  | <span data-ttu-id="f5ee8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f5ee8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ee8-126">Request body</span></span>
<span data-ttu-id="f5ee8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5ee8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ee8-128">Response</span></span>

<span data-ttu-id="f5ee8-129">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [Icon](../resources/icon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-129">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5ee8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5ee8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5ee8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ee8-131">Request</span></span>
<span data-ttu-id="f5ee8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="f5ee8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ee8-133">Response</span></span>
<span data-ttu-id="f5ee8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5ee8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->