---
title: Obtenha o grupo de roteamento de áudio
description: Recupere as propriedades e relacionamentos de um objeto audioRoutingGroup.
ms.openlocfilehash: ce1c8afea4932427a700970a16d3ec22a7f14d8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034674"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="b8f5f-103">Obtenha o grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="b8f5f-103">Get audio routing group</span></span>

> <span data-ttu-id="b8f5f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8f5f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8f5f-106">Recupere as propriedades e relacionamentos de um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b8f5f-106">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8f5f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b8f5f-107">Permissions</span></span>
<span data-ttu-id="b8f5f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8f5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8f5f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8f5f-110">Permission type</span></span>                        | <span data-ttu-id="b8f5f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8f5f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8f5f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8f5f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8f5f-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b8f5f-113">Not Supported</span></span>                               |
| <span data-ttu-id="b8f5f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8f5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8f5f-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b8f5f-115">Not Supported</span></span>                               |
| <span data-ttu-id="b8f5f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8f5f-116">Application</span></span>     | <span data-ttu-id="b8f5f-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b8f5f-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8f5f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8f5f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8f5f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8f5f-119">Optional query parameters</span></span>
<span data-ttu-id="b8f5f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8f5f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f5f-121">Request headers</span></span>
| <span data-ttu-id="b8f5f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b8f5f-122">Name</span></span>          | <span data-ttu-id="b8f5f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8f5f-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b8f5f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8f5f-124">Authorization</span></span> | <span data-ttu-id="b8f5f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8f5f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f5f-127">Request body</span></span>
<span data-ttu-id="b8f5f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8f5f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8f5f-129">Response</span></span>
<span data-ttu-id="b8f5f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-130">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8f5f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8f5f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8f5f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f5f-132">Request</span></span>
<span data-ttu-id="b8f5f-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="b8f5f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8f5f-134">Response</span></span>

> <span data-ttu-id="b8f5f-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8f5f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
