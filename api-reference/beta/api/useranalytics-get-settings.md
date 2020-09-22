---
title: Obter configurações para análise de usuário
description: Recupere as propriedades do objeto de configurações para a análise do usuário.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: eb88e2ca480a448bee5fe0c6ebc9f2cba0ee9d0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022068"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="bd6bb-103">Obter configurações para análise de usuário</span><span class="sxs-lookup"><span data-stu-id="bd6bb-103">Get settings for user analytics</span></span>

<span data-ttu-id="bd6bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd6bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6bb-105">Recupere as propriedades de um objeto de [configurações](../resources/settings.md) conforme aplicável para a API de análise.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd6bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd6bb-106">Permissions</span></span>

<span data-ttu-id="bd6bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd6bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd6bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd6bb-109">Permission type</span></span>                        | <span data-ttu-id="bd6bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd6bb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd6bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd6bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd6bb-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="bd6bb-112">User.Read</span></span> |
| <span data-ttu-id="bd6bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd6bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd6bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-114">Not supported.</span></span> |
| <span data-ttu-id="bd6bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd6bb-115">Application</span></span>                            | <span data-ttu-id="bd6bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd6bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd6bb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd6bb-118">Optional query parameters</span></span>

<span data-ttu-id="bd6bb-119">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd6bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6bb-120">Request headers</span></span>

| <span data-ttu-id="bd6bb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bd6bb-121">Name</span></span>      |<span data-ttu-id="bd6bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6bb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd6bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd6bb-123">Authorization</span></span> | <span data-ttu-id="bd6bb-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="bd6bb-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd6bb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6bb-125">Request body</span></span>

<span data-ttu-id="bd6bb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd6bb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6bb-127">Response</span></span>

<span data-ttu-id="bd6bb-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e o objeto de [configurações](../resources/settings.md) solicitadas no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd6bb-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd6bb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd6bb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6bb-130">Request</span></span>

<span data-ttu-id="bd6bb-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd6bb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6bb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="bd6bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="bd6bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd6bb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd6bb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd6bb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd6bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd6bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6bb-136">Response</span></span>

<span data-ttu-id="bd6bb-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd6bb-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.settings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('12ab2b12-4b1a-43a1-adac-1a123456cd78')/analytics/settings",
    "hasLicense": true,
    "hasOptedOut": false,
    "hasGraphMailbox": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


