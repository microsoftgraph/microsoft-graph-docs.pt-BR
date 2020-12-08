---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a82c03e9b63d83f8aab8b3556e75b17d926ff3e6
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581181"
---
# <a name="get-presence"></a><span data-ttu-id="43d11-103">Obter presença</span><span class="sxs-lookup"><span data-stu-id="43d11-103">Get presence</span></span>

<span data-ttu-id="43d11-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="43d11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43d11-105">Obtenha as informações de [presença](../resources/presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="43d11-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="43d11-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="43d11-106">Permissions</span></span>
<span data-ttu-id="43d11-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="43d11-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="43d11-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43d11-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43d11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43d11-109">Permission type</span></span> | <span data-ttu-id="43d11-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43d11-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="43d11-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43d11-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="43d11-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="43d11-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="43d11-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43d11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43d11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43d11-114">Not Supported.</span></span>                        |
| <span data-ttu-id="43d11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43d11-115">Application</span></span>                            | <span data-ttu-id="43d11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43d11-116">Not Supported.</span></span>                        |

> <span data-ttu-id="43d11-117">**Observação:** A taxa máxima de solicitações para esta API são 1500 solicitações de API em um período de 30 segundos, por aplicativo por locatário.</span><span class="sxs-lookup"><span data-stu-id="43d11-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="43d11-118">Solicitações HTTP</span><span class="sxs-lookup"><span data-stu-id="43d11-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="43d11-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43d11-119">Request Headers</span></span>
| <span data-ttu-id="43d11-120">Nome</span><span class="sxs-lookup"><span data-stu-id="43d11-120">Name</span></span>          | <span data-ttu-id="43d11-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="43d11-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="43d11-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43d11-122">Authorization</span></span> | <span data-ttu-id="43d11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43d11-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="43d11-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43d11-125">Request body</span></span>

<span data-ttu-id="43d11-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43d11-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43d11-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d11-127">Response</span></span>
<span data-ttu-id="43d11-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43d11-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43d11-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43d11-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="43d11-130">Exemplo 1: obter suas próprias informações de presença</span><span class="sxs-lookup"><span data-stu-id="43d11-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="43d11-131">O exemplo a seguir mostra como obter suas próprias informações de presença.</span><span class="sxs-lookup"><span data-stu-id="43d11-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="43d11-132">Esta operação requer a permissão Presence. Read.</span><span class="sxs-lookup"><span data-stu-id="43d11-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="43d11-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43d11-133">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```

---


#### <a name="response"></a><span data-ttu-id="43d11-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d11-134">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="43d11-135">Exemplo 2: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="43d11-135">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="43d11-136">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="43d11-136">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="43d11-137">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="43d11-137">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="43d11-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43d11-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

---


#### <a name="response"></a><span data-ttu-id="43d11-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d11-139">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="43d11-140">Exemplo 3: obter as informações de presença de outro usuário</span><span class="sxs-lookup"><span data-stu-id="43d11-140">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="43d11-141">O exemplo a seguir mostra como obter as informações de presença de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="43d11-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="43d11-142">Esta operação requer a permissão Presence. Read. All.</span><span class="sxs-lookup"><span data-stu-id="43d11-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="43d11-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43d11-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a><span data-ttu-id="43d11-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d11-144">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


