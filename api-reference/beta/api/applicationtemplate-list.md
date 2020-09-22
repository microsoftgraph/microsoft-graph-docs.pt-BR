---
title: Listar applicationTemplates
description: Recupere uma lista de objetos applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5df0ee457464e766fd2581bcb9440039029fc58a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996647"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="36483-103">Listar applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="36483-103">List applicationTemplates</span></span>

<span data-ttu-id="36483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36483-105">Recupere uma lista de objetos [applicationtemplate](../resources/applicationtemplate.md) da Galeria de aplicativos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36483-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="36483-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36483-106">Permissions</span></span>

<span data-ttu-id="36483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36483-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36483-109">Permission type</span></span>                        | <span data-ttu-id="36483-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36483-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36483-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36483-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36483-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36483-112">None.</span></span> |
| <span data-ttu-id="36483-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36483-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36483-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36483-114">Not supported.</span></span> |
| <span data-ttu-id="36483-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36483-115">Application</span></span>                            | <span data-ttu-id="36483-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36483-116">None.</span></span> |

<span data-ttu-id="36483-117">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="36483-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="36483-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36483-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36483-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36483-119">Optional query parameters</span></span>

<span data-ttu-id="36483-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36483-120">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="36483-121">Você pode usar o `$filter` parâmetro de forma limitada.</span><span class="sxs-lookup"><span data-stu-id="36483-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="36483-122">Você só pode filtrar por **DisplayName** ou **categorias**.</span><span class="sxs-lookup"><span data-stu-id="36483-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="36483-123">Por exemplo,  `$filter=contains(displayName, 'salesf')` ou `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="36483-123">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="36483-124">Você pode usar `$orderby` `$top,` e `$skip` consultar parâmetros em qualquer solicitação get.</span><span class="sxs-lookup"><span data-stu-id="36483-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="36483-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="36483-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36483-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36483-126">Request headers</span></span>

| <span data-ttu-id="36483-127">Nome</span><span class="sxs-lookup"><span data-stu-id="36483-127">Name</span></span>      |<span data-ttu-id="36483-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="36483-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36483-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="36483-129">Authorization</span></span> | <span data-ttu-id="36483-130">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="36483-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="36483-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36483-131">Request body</span></span>

<span data-ttu-id="36483-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36483-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36483-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="36483-133">Response</span></span>

<span data-ttu-id="36483-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [applicationtemplate](../resources/applicationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36483-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36483-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36483-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36483-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36483-136">Request</span></span>

<span data-ttu-id="36483-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36483-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36483-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="36483-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="36483-139">C#</span><span class="sxs-lookup"><span data-stu-id="36483-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36483-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36483-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36483-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36483-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36483-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="36483-142">Response</span></span>

<span data-ttu-id="36483-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36483-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="36483-144">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36483-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36483-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36483-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applicationTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


