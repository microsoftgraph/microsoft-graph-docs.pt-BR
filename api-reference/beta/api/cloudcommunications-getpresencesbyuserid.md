---
title: 'cloudCommunications: getPresencesByUserId'
description: Obtenha as informações de presença de vários usuários.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 256fdbbe86eb667fa06ca411aad050bf5e8013dc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912724"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="27643-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="27643-103">cloudCommunications: getPresencesByUserId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27643-104">Obtenha as informações de [presença](../resources/presence.md) de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="27643-104">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="27643-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27643-105">Permissions</span></span>
<span data-ttu-id="27643-106">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="27643-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="27643-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27643-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27643-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27643-108">Permission type</span></span> | <span data-ttu-id="27643-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27643-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="27643-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27643-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27643-111">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="27643-111">Presence.Read.All</span></span>                         |
| <span data-ttu-id="27643-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27643-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27643-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27643-113">Not Supported.</span></span>                         |
| <span data-ttu-id="27643-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27643-114">Application</span></span>                            | <span data-ttu-id="27643-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27643-115">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="27643-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27643-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="27643-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27643-117">Request Headers</span></span>
| <span data-ttu-id="27643-118">Nome</span><span class="sxs-lookup"><span data-stu-id="27643-118">Name</span></span>          | <span data-ttu-id="27643-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="27643-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="27643-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="27643-120">Authorization</span></span> | <span data-ttu-id="27643-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27643-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="27643-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="27643-123">Content-type</span></span> | <span data-ttu-id="27643-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27643-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="27643-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27643-126">Request body</span></span>

<span data-ttu-id="27643-127">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="27643-127">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="27643-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27643-128">Parameter</span></span>      | <span data-ttu-id="27643-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="27643-129">Type</span></span>    |<span data-ttu-id="27643-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="27643-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27643-131">ids</span><span class="sxs-lookup"><span data-stu-id="27643-131">ids</span></span>|<span data-ttu-id="27643-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="27643-132">String collection</span></span>|<span data-ttu-id="27643-133">As IDs de objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="27643-133">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="27643-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27643-134">Response</span></span>

<span data-ttu-id="27643-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Presence](../resources/presence.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27643-135">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="27643-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27643-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27643-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27643-137">Request</span></span>
<span data-ttu-id="27643-138">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="27643-138">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="27643-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="27643-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="27643-140">C#</span><span class="sxs-lookup"><span data-stu-id="27643-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27643-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27643-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27643-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27643-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="27643-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="27643-143">Response</span></span>
<span data-ttu-id="27643-144">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="27643-144">The following example shows the response.</span></span>

> <span data-ttu-id="27643-145">**Observação:** Os objetos Response podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="27643-145">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="27643-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27643-146">All the properties will be returned from an actual call.</span></span>

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
