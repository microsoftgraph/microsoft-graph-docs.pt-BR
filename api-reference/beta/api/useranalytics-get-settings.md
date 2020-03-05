---
title: Obter configurações para análise de usuário
description: Recupere as propriedades do objeto de configurações para a análise do usuário.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: be09792d08799d952334c33d52e0985196df7800
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451581"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="3e532-103">Obter configurações para análise de usuário</span><span class="sxs-lookup"><span data-stu-id="3e532-103">Get settings for user analytics</span></span>

<span data-ttu-id="3e532-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3e532-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e532-105">Recupere as propriedades de um objeto de [configurações](../resources/settings.md) conforme aplicável para a API de análise.</span><span class="sxs-lookup"><span data-stu-id="3e532-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e532-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e532-106">Permissions</span></span>

<span data-ttu-id="3e532-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e532-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e532-109">Permission type</span></span>                        | <span data-ttu-id="3e532-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e532-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e532-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e532-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e532-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="3e532-112">User.Read</span></span> |
| <span data-ttu-id="3e532-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e532-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e532-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e532-114">Not supported.</span></span> |
| <span data-ttu-id="3e532-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e532-115">Application</span></span>                            | <span data-ttu-id="3e532-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e532-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e532-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e532-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e532-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e532-118">Optional query parameters</span></span>

<span data-ttu-id="3e532-119">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e532-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e532-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e532-120">Request headers</span></span>

| <span data-ttu-id="3e532-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3e532-121">Name</span></span>      |<span data-ttu-id="3e532-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e532-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e532-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e532-123">Authorization</span></span> | <span data-ttu-id="3e532-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="3e532-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e532-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e532-125">Request body</span></span>

<span data-ttu-id="3e532-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e532-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e532-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e532-127">Response</span></span>

<span data-ttu-id="3e532-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e o objeto de [configurações](../resources/settings.md) solicitadas no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e532-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e532-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e532-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e532-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e532-130">Request</span></span>

<span data-ttu-id="3e532-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e532-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e532-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e532-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="3e532-133">C#</span><span class="sxs-lookup"><span data-stu-id="3e532-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e532-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e532-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e532-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e532-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e532-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e532-136">Response</span></span>

<span data-ttu-id="3e532-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e532-137">The following is an example of the response.</span></span>

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
