---
title: Obter perfil
description: Recupere as propriedades e os relacionamentos do objeto de perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5c9baff1dc69266fe6e58b747cfab051d7422f78
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997002"
---
# <a name="get-profile"></a><span data-ttu-id="9ad53-103">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="9ad53-103">Get profile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ad53-104">Recupere as propriedades e os relacionamentos de um objeto de [perfil](../resources/profile.md) para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="9ad53-104">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ad53-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ad53-105">Permissions</span></span>

<span data-ttu-id="9ad53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ad53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ad53-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ad53-108">Permission type</span></span>                        | <span data-ttu-id="9ad53-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ad53-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ad53-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ad53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ad53-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad53-111">Not supported.</span></span>                              |
| <span data-ttu-id="9ad53-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ad53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad53-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad53-113">Not supported.</span></span>                              |
| <span data-ttu-id="9ad53-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ad53-114">Application</span></span>                            | <span data-ttu-id="9ad53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad53-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="9ad53-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ad53-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ad53-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ad53-117">Optional query parameters</span></span>

<span data-ttu-id="9ad53-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ad53-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ad53-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ad53-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ad53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad53-120">Request headers</span></span>

| <span data-ttu-id="9ad53-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9ad53-121">Name</span></span>           |<span data-ttu-id="9ad53-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ad53-122">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="9ad53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ad53-123">Authorization</span></span>  | <span data-ttu-id="9ad53-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ad53-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9ad53-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ad53-126">Content-Type</span></span>   | <span data-ttu-id="9ad53-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ad53-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ad53-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad53-129">Request body</span></span>

<span data-ttu-id="9ad53-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ad53-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ad53-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ad53-131">Response</span></span>

<span data-ttu-id="9ad53-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto de [perfil](../resources/profile.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ad53-132">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ad53-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9ad53-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ad53-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad53-134">Request</span></span>

<span data-ttu-id="9ad53-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ad53-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ad53-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ad53-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ad53-137">C#</span><span class="sxs-lookup"><span data-stu-id="9ad53-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ad53-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ad53-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ad53-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ad53-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ad53-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ad53-140">Response</span></span>

<span data-ttu-id="9ad53-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ad53-141">The following is an example of the response.</span></span>

> <span data-ttu-id="9ad53-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ad53-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
