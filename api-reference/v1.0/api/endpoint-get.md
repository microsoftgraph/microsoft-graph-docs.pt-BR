---
title: Obter o ponto de extremidade
description: Recupere as propriedades e os relacionamentos de um objeto Endpoint específico.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 61afceb23471306962ef5dbea895b0b5e5d38c48
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289854"
---
# <a name="get-endpoint"></a><span data-ttu-id="e0e18-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="e0e18-103">Get endpoint</span></span>

<span data-ttu-id="e0e18-104">Recupere as propriedades e os relacionamentos de um objeto [Endpoint](../resources/endpoint.md) específico.</span><span class="sxs-lookup"><span data-stu-id="e0e18-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e18-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0e18-105">Permissions</span></span>
<span data-ttu-id="e0e18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0e18-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0e18-108">Permission type</span></span>      | <span data-ttu-id="e0e18-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0e18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0e18-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0e18-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0e18-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0e18-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0e18-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0e18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0e18-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0e18-113">Not supported.</span></span>    |
|<span data-ttu-id="e0e18-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0e18-114">Application</span></span> | <span data-ttu-id="e0e18-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0e18-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0e18-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e18-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0e18-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0e18-117">Optional query parameters</span></span>
<span data-ttu-id="e0e18-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e18-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0e18-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e18-119">Request headers</span></span>
| <span data-ttu-id="e0e18-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e0e18-120">Name</span></span>      |<span data-ttu-id="e0e18-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0e18-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0e18-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0e18-122">Authorization</span></span>  | <span data-ttu-id="e0e18-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0e18-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0e18-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e18-125">Request body</span></span>
<span data-ttu-id="e0e18-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0e18-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0e18-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e18-127">Response</span></span>

<span data-ttu-id="e0e18-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Endpoint](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e18-128">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0e18-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0e18-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0e18-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e18-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e0e18-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e18-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```

### <a name="response"></a><span data-ttu-id="e0e18-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e18-132">Response</span></span>
<span data-ttu-id="e0e18-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e18-133">Here is an example of the response.</span></span>
><span data-ttu-id="e0e18-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0e18-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
