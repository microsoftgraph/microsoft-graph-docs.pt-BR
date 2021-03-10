---
title: Obter ícone
description: Recupere as propriedades e os relacionamentos do objeto de ícone.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 2af12fcae9b26ca3aff994a1a89ddc089ee76fa8
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576754"
---
# <a name="get-icon"></a><span data-ttu-id="671fc-103">Get Icon</span><span class="sxs-lookup"><span data-stu-id="671fc-103">Get Icon</span></span>

<span data-ttu-id="671fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="671fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="671fc-105">Recupere as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="671fc-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="671fc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="671fc-106">Permissions</span></span>
<span data-ttu-id="671fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="671fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="671fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="671fc-109">Permission type</span></span>      | <span data-ttu-id="671fc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="671fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="671fc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="671fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="671fc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="671fc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="671fc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="671fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="671fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="671fc-114">Not supported.</span></span>    |
|<span data-ttu-id="671fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="671fc-115">Application</span></span> | <span data-ttu-id="671fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="671fc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="671fc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="671fc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="671fc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="671fc-118">Optional query parameters</span></span>
<span data-ttu-id="671fc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="671fc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="671fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="671fc-120">Request headers</span></span>
| <span data-ttu-id="671fc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="671fc-121">Name</span></span>      |<span data-ttu-id="671fc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="671fc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="671fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="671fc-123">Authorization</span></span>  | <span data-ttu-id="671fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="671fc-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="671fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="671fc-126">Request body</span></span>
<span data-ttu-id="671fc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="671fc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="671fc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="671fc-128">Response</span></span>

<span data-ttu-id="671fc-129">Se bem sucedido, este método retorna o código de resposta `200 OK` e o objeto [Icon](../resources/icon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="671fc-129">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="671fc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="671fc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="671fc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="671fc-131">Request</span></span>
<span data-ttu-id="671fc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="671fc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="671fc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="671fc-133">Response</span></span>
<span data-ttu-id="671fc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="671fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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