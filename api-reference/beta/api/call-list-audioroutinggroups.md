---
title: Grupos de roteamento áudio de lista
description: Recupere uma lista de objetos **audioRoutingGroup** .
ms.openlocfilehash: da6724f95fbc2c4365a1b1e4d34d317c130f12df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037674"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="c4591-103">Grupos de roteamento áudio de lista</span><span class="sxs-lookup"><span data-stu-id="c4591-103">List audio routing groups</span></span>

> <span data-ttu-id="c4591-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c4591-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4591-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c4591-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4591-106">Recupere uma lista de objetos **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="c4591-106">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4591-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c4591-107">Permissions</span></span>
<span data-ttu-id="c4591-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4591-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4591-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4591-110">Permission type</span></span>                        | <span data-ttu-id="c4591-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4591-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c4591-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4591-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4591-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="c4591-113">Not Supported.</span></span>                               |
| <span data-ttu-id="c4591-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4591-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4591-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="c4591-115">Not Supported.</span></span>                               |
| <span data-ttu-id="c4591-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4591-116">Application</span></span>     | <span data-ttu-id="c4591-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="c4591-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4591-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4591-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4591-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4591-119">Optional query parameters</span></span>
<span data-ttu-id="c4591-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4591-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4591-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4591-121">Request headers</span></span>
| <span data-ttu-id="c4591-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c4591-122">Name</span></span>          | <span data-ttu-id="c4591-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4591-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c4591-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4591-124">Authorization</span></span> | <span data-ttu-id="c4591-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4591-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4591-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4591-127">Request body</span></span>
<span data-ttu-id="c4591-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4591-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4591-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4591-129">Response</span></span>
<span data-ttu-id="c4591-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4591-130">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4591-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4591-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4591-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4591-132">Request</span></span>
<span data-ttu-id="c4591-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4591-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="c4591-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4591-134">Response</span></span>

> <span data-ttu-id="c4591-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4591-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
    {
      "id": "oneToOne",
      "routingMode": "oneToOne",
      "sources": [
        "632899f8-2ea1-4604-8413-27bd2892079f"
      ],
      "receivers": [
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
