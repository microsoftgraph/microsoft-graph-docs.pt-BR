---
title: Obtenha o grupo de roteamento de áudio
description: Recupere as propriedades e relacionamentos de um objeto audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 08c86e0a88cb77ddf42f8b7feee2f55093723d35
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922554"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="43ac8-103">Obtenha o grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="43ac8-103">Get audio routing group</span></span>

> <span data-ttu-id="43ac8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43ac8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43ac8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43ac8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43ac8-106">Recupere as propriedades e relacionamentos de um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="43ac8-106">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43ac8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="43ac8-107">Permissions</span></span>
<span data-ttu-id="43ac8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43ac8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43ac8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43ac8-110">Permission type</span></span>                        | <span data-ttu-id="43ac8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43ac8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="43ac8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43ac8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="43ac8-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="43ac8-113">Not Supported</span></span>                               |
| <span data-ttu-id="43ac8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43ac8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43ac8-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="43ac8-115">Not Supported</span></span>                               |
| <span data-ttu-id="43ac8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43ac8-116">Application</span></span>                            | <span data-ttu-id="43ac8-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="43ac8-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43ac8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43ac8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43ac8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43ac8-119">Optional query parameters</span></span>
<span data-ttu-id="43ac8-120">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43ac8-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43ac8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43ac8-121">Request headers</span></span>
| <span data-ttu-id="43ac8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="43ac8-122">Name</span></span>          | <span data-ttu-id="43ac8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="43ac8-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="43ac8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="43ac8-124">Authorization</span></span> | <span data-ttu-id="43ac8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43ac8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43ac8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43ac8-127">Request body</span></span>
<span data-ttu-id="43ac8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43ac8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43ac8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="43ac8-129">Response</span></span>
<span data-ttu-id="43ac8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43ac8-130">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43ac8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43ac8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="43ac8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43ac8-132">Request</span></span>
<span data-ttu-id="43ac8-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="43ac8-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="43ac8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="43ac8-134">Response</span></span>

> <span data-ttu-id="43ac8-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43ac8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
