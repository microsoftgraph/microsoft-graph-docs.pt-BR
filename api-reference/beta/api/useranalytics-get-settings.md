---
title: Obter configurações para análise de usuário
description: Recupere as propriedades do objeto de configurações para a análise do usuário.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: dac1a97ea0a2889b26b305ddd6c3fd3e038b7d93
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461557"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="73fa8-103">Obter configurações para análise de usuário</span><span class="sxs-lookup"><span data-stu-id="73fa8-103">Get settings for user analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73fa8-104">Recupere as propriedades de um objeto de [configurações](../resources/settings.md) conforme aplicável para a API de análise.</span><span class="sxs-lookup"><span data-stu-id="73fa8-104">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="73fa8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="73fa8-105">Permissions</span></span>

<span data-ttu-id="73fa8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73fa8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73fa8-108">Permission type</span></span>                        | <span data-ttu-id="73fa8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73fa8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73fa8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73fa8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="73fa8-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="73fa8-111">User.Read</span></span> |
| <span data-ttu-id="73fa8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73fa8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73fa8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73fa8-113">Not supported.</span></span> |
| <span data-ttu-id="73fa8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73fa8-114">Application</span></span>                            | <span data-ttu-id="73fa8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73fa8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73fa8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73fa8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET https://graph.microsoft.com/beta/me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73fa8-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73fa8-117">Optional query parameters</span></span>

<span data-ttu-id="73fa8-118">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73fa8-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73fa8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73fa8-119">Request headers</span></span>

| <span data-ttu-id="73fa8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="73fa8-120">Name</span></span>      |<span data-ttu-id="73fa8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="73fa8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73fa8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73fa8-122">Authorization</span></span> | <span data-ttu-id="73fa8-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="73fa8-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="73fa8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73fa8-124">Request body</span></span>

<span data-ttu-id="73fa8-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73fa8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73fa8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="73fa8-126">Response</span></span>

<span data-ttu-id="73fa8-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e o objeto de [configurações](../resources/settings.md) solicitadas no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73fa8-127">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73fa8-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73fa8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73fa8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73fa8-129">Request</span></span>

<span data-ttu-id="73fa8-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73fa8-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73fa8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="73fa8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73fa8-132">C#</span><span class="sxs-lookup"><span data-stu-id="73fa8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73fa8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73fa8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73fa8-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="73fa8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73fa8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="73fa8-135">Response</span></span>

<span data-ttu-id="73fa8-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73fa8-136">The following is an example of the response.</span></span>

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
