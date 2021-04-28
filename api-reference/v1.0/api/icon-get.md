---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8c05b0c9733515f80db0189e6f9cb7bbee6a0fd8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050441"
---
# <a name="get-icon"></a><span data-ttu-id="e5de6-103">Get Icon</span><span class="sxs-lookup"><span data-stu-id="e5de6-103">Get Icon</span></span>

<span data-ttu-id="e5de6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5de6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5de6-105">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="e5de6-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5de6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5de6-106">Permissions</span></span>
<span data-ttu-id="e5de6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5de6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5de6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5de6-109">Permission type</span></span>      | <span data-ttu-id="e5de6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5de6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5de6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5de6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5de6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5de6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5de6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5de6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5de6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5de6-114">Not supported.</span></span>    |
|<span data-ttu-id="e5de6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5de6-115">Application</span></span> | <span data-ttu-id="e5de6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5de6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5de6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5de6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5de6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5de6-118">Optional query parameters</span></span>
<span data-ttu-id="e5de6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e5de6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5de6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5de6-120">Request headers</span></span>
| <span data-ttu-id="e5de6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e5de6-121">Name</span></span>      |<span data-ttu-id="e5de6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5de6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5de6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5de6-123">Authorization</span></span>  | <span data-ttu-id="e5de6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5de6-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e5de6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5de6-126">Request body</span></span>
<span data-ttu-id="e5de6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5de6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5de6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5de6-128">Response</span></span>

<span data-ttu-id="e5de6-129">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [Icon](../resources/icon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5de6-129">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5de6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5de6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5de6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5de6-131">Request</span></span>
<span data-ttu-id="e5de6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5de6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="e5de6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5de6-133">Response</span></span>
<span data-ttu-id="e5de6-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5de6-134">Here is an example of the response.</span></span> <span data-ttu-id="e5de6-135">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5de6-135">Note: The response object shown here might be shortened for readability.</span></span>
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