---
title: Obter perfil
description: Recupere as propriedades e os relacionamentos do objeto de perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d0bc20c6e83f8f2bd9e67268eb9471d84bbdcb16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455239"
---
# <a name="get-profile"></a><span data-ttu-id="37553-103">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="37553-103">Get profile</span></span>

<span data-ttu-id="37553-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37553-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37553-105">Recupere as propriedades e os relacionamentos de um objeto de [perfil](../resources/profile.md) para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="37553-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="37553-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37553-106">Permissions</span></span>

<span data-ttu-id="37553-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37553-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37553-109">Permission type</span></span>                        | <span data-ttu-id="37553-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37553-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37553-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37553-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37553-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37553-112">Not supported.</span></span>                              |
| <span data-ttu-id="37553-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37553-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37553-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37553-114">Not supported.</span></span>                              |
| <span data-ttu-id="37553-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37553-115">Application</span></span>                            | <span data-ttu-id="37553-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37553-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="37553-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37553-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37553-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37553-118">Optional query parameters</span></span>

<span data-ttu-id="37553-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37553-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="37553-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="37553-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37553-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37553-121">Request headers</span></span>

| <span data-ttu-id="37553-122">Nome</span><span class="sxs-lookup"><span data-stu-id="37553-122">Name</span></span>           |<span data-ttu-id="37553-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="37553-123">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="37553-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="37553-124">Authorization</span></span>  | <span data-ttu-id="37553-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37553-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="37553-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37553-127">Content-Type</span></span>   | <span data-ttu-id="37553-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37553-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37553-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37553-130">Request body</span></span>

<span data-ttu-id="37553-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37553-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37553-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="37553-132">Response</span></span>

<span data-ttu-id="37553-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto de [perfil](../resources/profile.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37553-133">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37553-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37553-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37553-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37553-135">Request</span></span>

<span data-ttu-id="37553-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37553-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37553-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="37553-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="37553-138">C#</span><span class="sxs-lookup"><span data-stu-id="37553-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37553-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37553-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37553-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37553-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37553-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="37553-141">Response</span></span>

<span data-ttu-id="37553-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37553-142">The following is an example of the response.</span></span>

> <span data-ttu-id="37553-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37553-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
