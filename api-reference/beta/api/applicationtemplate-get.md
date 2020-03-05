---
title: Obter applicationtemplate
description: Recupere as propriedades e os relacionamentos do objeto applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbf38412fc6442ffcc0a7037e2a1dcde30a35469
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441400"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="7f492-103">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="7f492-103">Get applicationTemplate</span></span>

<span data-ttu-id="7f492-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f492-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f492-105">Recupere as propriedades de um objeto [applicationtemplate](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="7f492-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f492-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f492-106">Permissions</span></span>

<span data-ttu-id="7f492-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f492-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f492-109">Permission type</span></span>                        | <span data-ttu-id="7f492-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f492-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f492-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f492-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f492-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7f492-112">None.</span></span> |
| <span data-ttu-id="7f492-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f492-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f492-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f492-114">Not supported.</span></span> |
| <span data-ttu-id="7f492-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f492-115">Application</span></span>                            | <span data-ttu-id="7f492-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7f492-116">None.</span></span> |

<span data-ttu-id="7f492-117">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7f492-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f492-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f492-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f492-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f492-119">Optional query parameters</span></span>

<span data-ttu-id="7f492-120">Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades que você precisa para o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="7f492-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="7f492-121">A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="7f492-121">The **id** property is always returned.</span></span> 

<span data-ttu-id="7f492-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7f492-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f492-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f492-123">Request headers</span></span>

| <span data-ttu-id="7f492-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7f492-124">Name</span></span>      |<span data-ttu-id="7f492-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f492-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f492-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f492-126">Authorization</span></span> | <span data-ttu-id="7f492-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7f492-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f492-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f492-128">Request body</span></span>

<span data-ttu-id="7f492-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f492-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f492-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f492-130">Response</span></span>

<span data-ttu-id="7f492-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [applicationtemplate](../resources/applicationtemplate.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f492-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f492-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7f492-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f492-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f492-133">Request</span></span>

<span data-ttu-id="7f492-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f492-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f492-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f492-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="7f492-136">C#</span><span class="sxs-lookup"><span data-stu-id="7f492-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f492-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f492-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f492-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f492-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f492-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f492-139">Response</span></span>

<span data-ttu-id="7f492-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f492-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7f492-141">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f492-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f492-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f492-142">All the properties will be returned from an actual call.</span></span>

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
