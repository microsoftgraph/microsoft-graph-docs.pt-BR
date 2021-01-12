---
title: 'cloudCommunications: getPresencesByUserId'
description: Obter as informações de presença para vários usuários.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a3c6b0fe4d223ef458aad7d9b271cfdee37e590c
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796525"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="264b6-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="264b6-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="264b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="264b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="264b6-105">Obter as [informações de](../resources/presence.md) presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="264b6-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="264b6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="264b6-106">Permissions</span></span>
<span data-ttu-id="264b6-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="264b6-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="264b6-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264b6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="264b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="264b6-109">Permission type</span></span> | <span data-ttu-id="264b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="264b6-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="264b6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="264b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="264b6-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="264b6-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="264b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="264b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="264b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264b6-114">Not Supported.</span></span>                         |
| <span data-ttu-id="264b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="264b6-115">Application</span></span>                            | <span data-ttu-id="264b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264b6-116">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="264b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="264b6-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="264b6-118">Solicitação de headers</span><span class="sxs-lookup"><span data-stu-id="264b6-118">Request Headers</span></span>
| <span data-ttu-id="264b6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="264b6-119">Name</span></span>          | <span data-ttu-id="264b6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="264b6-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="264b6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="264b6-121">Authorization</span></span> | <span data-ttu-id="264b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="264b6-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="264b6-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="264b6-124">Content-type</span></span> | <span data-ttu-id="264b6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="264b6-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="264b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="264b6-127">Request body</span></span>

<span data-ttu-id="264b6-128">No corpo da solicitação, forneça um objeto JSON com o parâmetro a seguir.</span><span class="sxs-lookup"><span data-stu-id="264b6-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="264b6-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="264b6-129">Parameter</span></span>      | <span data-ttu-id="264b6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="264b6-130">Type</span></span>    |<span data-ttu-id="264b6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="264b6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="264b6-132">ids</span><span class="sxs-lookup"><span data-stu-id="264b6-132">ids</span></span>|<span data-ttu-id="264b6-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="264b6-133">String collection</span></span>|<span data-ttu-id="264b6-134">As IDs de objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="264b6-134">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="264b6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="264b6-135">Response</span></span>

<span data-ttu-id="264b6-136">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de objetos [de](../resources/presence.md) presença no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="264b6-136">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="264b6-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="264b6-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="264b6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="264b6-138">Request</span></span>
<span data-ttu-id="264b6-139">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="264b6-139">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="264b6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="264b6-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="264b6-141">C#</span><span class="sxs-lookup"><span data-stu-id="264b6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="264b6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="264b6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="264b6-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="264b6-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="264b6-144">Java</span><span class="sxs-lookup"><span data-stu-id="264b6-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="264b6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="264b6-145">Response</span></span>
<span data-ttu-id="264b6-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="264b6-146">The following example shows the response.</span></span>

> <span data-ttu-id="264b6-147">**Observação:** Os objetos de resposta podem ser reduzidos para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="264b6-147">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="264b6-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="264b6-148">All the properties will be returned from an actual call.</span></span>

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
      "activity": "InAMeeting",
      "outOfOfficeSettings": {
        "message": null,
        "isOutOfOffice": false
      }
    },
    {
      "id": "66825e03-7ef5-42da-9069-724602c31f6b",
      "availability": "Away",
      "activity": "Away",
      "outOfOfficeSettings": {
        "message": null,
        "isOutOfOffice": true
      }
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


