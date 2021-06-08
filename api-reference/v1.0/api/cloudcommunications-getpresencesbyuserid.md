---
title: 'cloudCommunications: getPresencesByUserId'
description: Obter informações de presença para vários usuários.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 61ce51d3fe7d85c2a5d086938c38f45827c2515e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787643"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="4632f-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="4632f-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="4632f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4632f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4632f-105">Obter informações [de](../resources/presence.md) presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="4632f-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="4632f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4632f-106">Permissions</span></span>
<span data-ttu-id="4632f-107">Uma das seguintes permissões é necessária para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="4632f-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="4632f-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4632f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4632f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4632f-109">Permission type</span></span> | <span data-ttu-id="4632f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4632f-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="4632f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4632f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4632f-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4632f-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="4632f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4632f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4632f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4632f-114">Not Supported.</span></span>                         |
| <span data-ttu-id="4632f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4632f-115">Application</span></span>                            | <span data-ttu-id="4632f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4632f-116">Not Supported.</span></span>                                  |

> <span data-ttu-id="4632f-117">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="4632f-117">**Note:**</span></span>
> * <span data-ttu-id="4632f-118">Há suporte para no máximo 650 IDs de usuário por solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="4632f-118">Maximum of 650 user IDs are supported per API request.</span></span>
> * <span data-ttu-id="4632f-119">A taxa máxima de solicitação dessa API é de 1500 solicitações de API em um período de 30 segundos, por aplicativo por locatário.</span><span class="sxs-lookup"><span data-stu-id="4632f-119">The maximum request rate of this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="4632f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4632f-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="4632f-121">Headers de solicitação</span><span class="sxs-lookup"><span data-stu-id="4632f-121">Request Headers</span></span>
| <span data-ttu-id="4632f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4632f-122">Name</span></span>          | <span data-ttu-id="4632f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4632f-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4632f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4632f-124">Authorization</span></span> | <span data-ttu-id="4632f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4632f-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="4632f-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="4632f-127">Content-type</span></span> | <span data-ttu-id="4632f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4632f-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4632f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4632f-130">Request body</span></span>

<span data-ttu-id="4632f-131">No corpo da solicitação, forneça um objeto JSON com o parâmetro a seguir.</span><span class="sxs-lookup"><span data-stu-id="4632f-131">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="4632f-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4632f-132">Parameter</span></span>      | <span data-ttu-id="4632f-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4632f-133">Type</span></span>    |<span data-ttu-id="4632f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4632f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4632f-135">ids</span><span class="sxs-lookup"><span data-stu-id="4632f-135">ids</span></span>|<span data-ttu-id="4632f-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4632f-136">String collection</span></span>|<span data-ttu-id="4632f-137">As IDs de objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="4632f-137">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="4632f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4632f-138">Response</span></span>

<span data-ttu-id="4632f-139">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/presence.md) presença no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4632f-139">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="4632f-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4632f-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4632f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4632f-141">Request</span></span>
<span data-ttu-id="4632f-142">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="4632f-142">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4632f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4632f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[<span data-ttu-id="4632f-144">C#</span><span class="sxs-lookup"><span data-stu-id="4632f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4632f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4632f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4632f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4632f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4632f-147">Java</span><span class="sxs-lookup"><span data-stu-id="4632f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="4632f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4632f-148">Response</span></span>
<span data-ttu-id="4632f-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="4632f-149">The following example shows the response.</span></span>

> <span data-ttu-id="4632f-150">**Observação:** Os objetos de resposta podem ser reduzidos para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="4632f-150">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="4632f-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4632f-151">All the properties will be returned from an actual call.</span></span>

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


