---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6ad126aa04f1d977ad065a9baaa2ce2cc2a72065
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014449"
---
# <a name="get-icon"></a><span data-ttu-id="c5245-103">Obter ícone</span><span class="sxs-lookup"><span data-stu-id="c5245-103">Get Icon</span></span>

<span data-ttu-id="c5245-104">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="c5245-104">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5245-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5245-105">Permissions</span></span>
<span data-ttu-id="c5245-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5245-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5245-108">Permission type</span></span>      | <span data-ttu-id="c5245-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5245-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c5245-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5245-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5245-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5245-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="c5245-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5245-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5245-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5245-113">Not supported.</span></span>    | 
|<span data-ttu-id="c5245-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5245-114">Application</span></span> | <span data-ttu-id="c5245-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5245-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c5245-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5245-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5245-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5245-117">Optional query parameters</span></span>
<span data-ttu-id="c5245-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5245-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5245-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5245-119">Request headers</span></span>
| <span data-ttu-id="c5245-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c5245-120">Name</span></span>      |<span data-ttu-id="c5245-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5245-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5245-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5245-122">Authorization</span></span>  | <span data-ttu-id="c5245-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5245-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c5245-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5245-125">Request body</span></span>
<span data-ttu-id="c5245-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5245-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5245-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5245-127">Response</span></span>

<span data-ttu-id="c5245-128">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [Icon](../resources/icon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5245-128">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5245-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5245-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5245-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5245-130">Request</span></span>
<span data-ttu-id="c5245-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5245-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="c5245-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5245-132">Response</span></span>
<span data-ttu-id="c5245-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5245-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
