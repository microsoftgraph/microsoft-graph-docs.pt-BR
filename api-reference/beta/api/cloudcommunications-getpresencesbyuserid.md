---
title: 'cloudCommunications: getPresencesByUserId'
description: Obtenha as informações de presença de vários usuários.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 7d670db030a1110bb0aa9844820f53814d9b1a82
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957985"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="77f7e-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="77f7e-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="77f7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f7e-105">Obtenha as informações de [presença](../resources/presence.md) de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="77f7e-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="77f7e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77f7e-106">Permissions</span></span>
<span data-ttu-id="77f7e-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="77f7e-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="77f7e-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f7e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77f7e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77f7e-109">Permission type</span></span> | <span data-ttu-id="77f7e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77f7e-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="77f7e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77f7e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77f7e-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="77f7e-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="77f7e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77f7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77f7e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77f7e-114">Not Supported.</span></span>                         |
| <span data-ttu-id="77f7e-115">Application</span><span class="sxs-lookup"><span data-stu-id="77f7e-115">Application</span></span>                            | <span data-ttu-id="77f7e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77f7e-116">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="77f7e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77f7e-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="77f7e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77f7e-118">Request Headers</span></span>
| <span data-ttu-id="77f7e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="77f7e-119">Name</span></span>          | <span data-ttu-id="77f7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f7e-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="77f7e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77f7e-121">Authorization</span></span> | <span data-ttu-id="77f7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f7e-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="77f7e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="77f7e-124">Content-type</span></span> | <span data-ttu-id="77f7e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f7e-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="77f7e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77f7e-127">Request body</span></span>

<span data-ttu-id="77f7e-128">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="77f7e-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="77f7e-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77f7e-129">Parameter</span></span>      | <span data-ttu-id="77f7e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="77f7e-130">Type</span></span>    |<span data-ttu-id="77f7e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f7e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f7e-132">ids</span><span class="sxs-lookup"><span data-stu-id="77f7e-132">ids</span></span>|<span data-ttu-id="77f7e-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="77f7e-133">String collection</span></span>|<span data-ttu-id="77f7e-134">As IDs de objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="77f7e-134">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="77f7e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f7e-135">Response</span></span>

<span data-ttu-id="77f7e-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77f7e-136">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="77f7e-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="77f7e-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77f7e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77f7e-138">Request</span></span>
<span data-ttu-id="77f7e-139">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="77f7e-139">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="77f7e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="77f7e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[<span data-ttu-id="77f7e-141">C#</span><span class="sxs-lookup"><span data-stu-id="77f7e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77f7e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77f7e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77f7e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77f7e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77f7e-144">Java</span><span class="sxs-lookup"><span data-stu-id="77f7e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="77f7e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f7e-145">Response</span></span>
<span data-ttu-id="77f7e-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="77f7e-146">The following example shows the response.</span></span>

> <span data-ttu-id="77f7e-147">**Observação:** Os objetos Response podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="77f7e-147">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="77f7e-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77f7e-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


