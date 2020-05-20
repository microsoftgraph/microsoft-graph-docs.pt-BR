---
title: Listar pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 738ccf502398a419dc54c12824cf6ce53654372e
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290410"
---
# <a name="list-endpoints"></a><span data-ttu-id="b8706-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="b8706-103">List endpoints</span></span>

<span data-ttu-id="b8706-104">Recupere uma lista de objetos de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="b8706-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8706-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8706-105">Permissions</span></span>
<span data-ttu-id="b8706-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8706-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8706-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8706-108">Permission type</span></span>      | <span data-ttu-id="b8706-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8706-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8706-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8706-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8706-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8706-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8706-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8706-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8706-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8706-113">Not supported.</span></span>    |
|<span data-ttu-id="b8706-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8706-114">Application</span></span> | <span data-ttu-id="b8706-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8706-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8706-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8706-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8706-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8706-117">Optional query parameters</span></span>
<span data-ttu-id="b8706-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8706-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8706-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8706-119">Request headers</span></span>
| <span data-ttu-id="b8706-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b8706-120">Name</span></span>      |<span data-ttu-id="b8706-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8706-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8706-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8706-122">Authorization</span></span>  | <span data-ttu-id="b8706-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8706-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b8706-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8706-125">Content-Type</span></span>   | <span data-ttu-id="b8706-126">Application/JSON</span><span class="sxs-lookup"><span data-stu-id="b8706-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8706-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8706-127">Request body</span></span>
<span data-ttu-id="b8706-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8706-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8706-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8706-129">Response</span></span>

<span data-ttu-id="b8706-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8706-130">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8706-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8706-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8706-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8706-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b8706-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8706-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```

### <a name="response"></a><span data-ttu-id="b8706-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8706-134">Response</span></span>
<span data-ttu-id="b8706-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8706-135">Here is an example of the response.</span></span>
><span data-ttu-id="b8706-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8706-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
