---
title: Obter applicationtemplate
description: Recupere as propriedades e os relacionamentos do objeto applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f18fcc9ca8255d7edbc4145d6d47783db13d52ba
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408165"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="7daf7-103">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="7daf7-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7daf7-104">Recupere as propriedades de um [](../resources/applicationtemplate.md) objeto applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="7daf7-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7daf7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7daf7-105">Permissions</span></span>

<span data-ttu-id="7daf7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7daf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7daf7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7daf7-108">Permission type</span></span>                        | <span data-ttu-id="7daf7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7daf7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7daf7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7daf7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7daf7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7daf7-111">None.</span></span> |
| <span data-ttu-id="7daf7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7daf7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7daf7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7daf7-113">Not supported.</span></span> |
| <span data-ttu-id="7daf7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7daf7-114">Application</span></span>                            | <span data-ttu-id="7daf7-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7daf7-115">None.</span></span> |

<span data-ttu-id="7daf7-116">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7daf7-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="7daf7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7daf7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7daf7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7daf7-118">Optional query parameters</span></span>

<span data-ttu-id="7daf7-119">Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades que você precisa para o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="7daf7-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="7daf7-120">A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="7daf7-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="7daf7-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7daf7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7daf7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7daf7-122">Request headers</span></span>

| <span data-ttu-id="7daf7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7daf7-123">Name</span></span>      |<span data-ttu-id="7daf7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7daf7-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7daf7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7daf7-125">Authorization</span></span> | <span data-ttu-id="7daf7-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7daf7-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7daf7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7daf7-127">Request body</span></span>

<span data-ttu-id="7daf7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7daf7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7daf7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7daf7-129">Response</span></span>

<span data-ttu-id="7daf7-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [applicationtemplate](../resources/applicationtemplate.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7daf7-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7daf7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7daf7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7daf7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7daf7-132">Request</span></span>

<span data-ttu-id="7daf7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7daf7-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7daf7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7daf7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7daf7-135">C#</span><span class="sxs-lookup"><span data-stu-id="7daf7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7daf7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7daf7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7daf7-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7daf7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7daf7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7daf7-138">Response</span></span>

<span data-ttu-id="7daf7-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7daf7-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7daf7-140">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7daf7-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7daf7-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7daf7-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
