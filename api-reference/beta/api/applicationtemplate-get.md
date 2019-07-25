---
title: Obter applicationtemplate
description: Recupere as propriedades e os relacionamentos do objeto applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58c7be5c341771e0c60010371064cc4510c88d5a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856691"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="678fe-103">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="678fe-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="678fe-104">Recupere as propriedades de um [](../resources/applicationtemplate.md) objeto applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="678fe-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="678fe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="678fe-105">Permissions</span></span>

<span data-ttu-id="678fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="678fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="678fe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="678fe-108">Permission type</span></span>                        | <span data-ttu-id="678fe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="678fe-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="678fe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="678fe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="678fe-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="678fe-111">None.</span></span> |
| <span data-ttu-id="678fe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="678fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="678fe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="678fe-113">Not supported.</span></span> |
| <span data-ttu-id="678fe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="678fe-114">Application</span></span>                            | <span data-ttu-id="678fe-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="678fe-115">None.</span></span> |

<span data-ttu-id="678fe-116">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="678fe-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="678fe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="678fe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="678fe-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="678fe-118">Optional query parameters</span></span>

<span data-ttu-id="678fe-119">Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades que você precisa para o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="678fe-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="678fe-120">A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="678fe-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="678fe-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="678fe-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="678fe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="678fe-122">Request headers</span></span>

| <span data-ttu-id="678fe-123">Nome</span><span class="sxs-lookup"><span data-stu-id="678fe-123">Name</span></span>      |<span data-ttu-id="678fe-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="678fe-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="678fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="678fe-125">Authorization</span></span> | <span data-ttu-id="678fe-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="678fe-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="678fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="678fe-127">Request body</span></span>

<span data-ttu-id="678fe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="678fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="678fe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="678fe-129">Response</span></span>

<span data-ttu-id="678fe-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [applicationtemplate](../resources/applicationtemplate.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="678fe-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="678fe-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="678fe-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="678fe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="678fe-132">Request</span></span>

<span data-ttu-id="678fe-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="678fe-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="678fe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="678fe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="678fe-135">C#</span><span class="sxs-lookup"><span data-stu-id="678fe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="678fe-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="678fe-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="678fe-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="678fe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="678fe-138">Java</span><span class="sxs-lookup"><span data-stu-id="678fe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="678fe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="678fe-139">Response</span></span>

<span data-ttu-id="678fe-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="678fe-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="678fe-141">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="678fe-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="678fe-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="678fe-142">All the properties will be returned from an actual call.</span></span>

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
