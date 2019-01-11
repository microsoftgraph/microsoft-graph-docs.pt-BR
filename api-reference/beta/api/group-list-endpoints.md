---
title: Lista de pontos de extremidade
description: Recupere uma lista de objetos de ponto de extremidade.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: ce208e34cd4d8401d537a36626eeefc7cb5ae126
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833261"
---
# <a name="list-endpoints"></a><span data-ttu-id="40e96-103">Lista de pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="40e96-103">List endpoints</span></span>

> <span data-ttu-id="40e96-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="40e96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40e96-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40e96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40e96-106">Recupere uma lista de objetos de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="40e96-106">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="40e96-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="40e96-107">Permissions</span></span>
<span data-ttu-id="40e96-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40e96-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40e96-110">Permission type</span></span>      | <span data-ttu-id="40e96-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40e96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40e96-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40e96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40e96-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40e96-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40e96-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40e96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40e96-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40e96-115">Not supported.</span></span>    |
|<span data-ttu-id="40e96-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40e96-116">Application</span></span> | <span data-ttu-id="40e96-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40e96-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40e96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40e96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40e96-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40e96-119">Optional query parameters</span></span>
<span data-ttu-id="40e96-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40e96-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40e96-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40e96-121">Request headers</span></span>
| <span data-ttu-id="40e96-122">Nome</span><span class="sxs-lookup"><span data-stu-id="40e96-122">Name</span></span>      |<span data-ttu-id="40e96-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="40e96-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40e96-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="40e96-124">Authorization</span></span>  | <span data-ttu-id="40e96-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40e96-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="40e96-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40e96-127">Content-Type</span></span>   | <span data-ttu-id="40e96-128">Application/Json</span><span class="sxs-lookup"><span data-stu-id="40e96-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="40e96-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40e96-129">Request body</span></span>
<span data-ttu-id="40e96-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40e96-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40e96-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40e96-131">Response</span></span>

<span data-ttu-id="40e96-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40e96-132">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40e96-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40e96-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40e96-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40e96-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="40e96-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="40e96-135">Response</span></span>
<span data-ttu-id="40e96-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40e96-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint",
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
<!-- {
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
