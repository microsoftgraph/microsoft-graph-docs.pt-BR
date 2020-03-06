---
title: Obter canal
description: Recuperar as propriedades e os relacionamentos de um canal.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9aa260dfe054c05f80cc0c53c9a2b8a4a10779c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518613"
---
# <a name="get-channel"></a><span data-ttu-id="b513e-103">Obter canal</span><span class="sxs-lookup"><span data-stu-id="b513e-103">Get channel</span></span>

<span data-ttu-id="b513e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b513e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b513e-105">Recuperar as propriedades e os relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b513e-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b513e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b513e-106">Permissions</span></span>
<span data-ttu-id="b513e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b513e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b513e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b513e-109">Permission type</span></span>      | <span data-ttu-id="b513e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b513e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b513e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b513e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b513e-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b513e-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b513e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b513e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b513e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b513e-114">Not supported.</span></span>    |
|<span data-ttu-id="b513e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b513e-115">Application</span></span> | <span data-ttu-id="b513e-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b513e-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="b513e-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="b513e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b513e-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="b513e-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b513e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b513e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="b513e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b513e-120">Optional query parameters</span></span>

<span data-ttu-id="b513e-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b513e-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b513e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b513e-122">Request headers</span></span>
| <span data-ttu-id="b513e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b513e-123">Header</span></span>       | <span data-ttu-id="b513e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b513e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b513e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b513e-125">Authorization</span></span>  | <span data-ttu-id="b513e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b513e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b513e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b513e-128">Request body</span></span>
<span data-ttu-id="b513e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b513e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b513e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b513e-130">Response</span></span>

<span data-ttu-id="b513e-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b513e-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b513e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b513e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b513e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b513e-133">Request</span></span>
<span data-ttu-id="b513e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b513e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b513e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b513e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="b513e-136">C#</span><span class="sxs-lookup"><span data-stu-id="b513e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b513e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b513e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b513e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b513e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b513e-139">Java</span><span class="sxs-lookup"><span data-stu-id="b513e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b513e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b513e-140">Response</span></span>
<span data-ttu-id="b513e-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b513e-141">Here is an example of the response.</span></span> 

><span data-ttu-id="b513e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b513e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
