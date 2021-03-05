---
title: Listar applicationTemplates
description: Recupere uma lista de objetos applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ebd1b178ad1a6ea0e178ab582439ace433951ffb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471530"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="e9505-103">Listar applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="e9505-103">List applicationTemplates</span></span>

<span data-ttu-id="e9505-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9505-105">Recupere uma lista de [objetos applicationTemplate](../resources/applicationtemplate.md) da galeria de aplicativos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9505-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9505-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9505-106">Permissions</span></span>

<span data-ttu-id="e9505-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9505-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9505-109">Permission type</span></span>                        | <span data-ttu-id="e9505-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9505-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9505-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9505-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9505-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9505-112">None.</span></span> |
| <span data-ttu-id="e9505-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9505-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9505-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9505-114">Not supported.</span></span> |
| <span data-ttu-id="e9505-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9505-115">Application</span></span>                            | <span data-ttu-id="e9505-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9505-116">None.</span></span> |

<span data-ttu-id="e9505-117">Permissões adicionais não são necessárias para chamar essa API, desde que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e9505-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9505-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9505-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9505-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9505-119">Optional query parameters</span></span>

<span data-ttu-id="e9505-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9505-120">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="e9505-121">Você pode usar o `$filter` parâmetro de forma limitada.</span><span class="sxs-lookup"><span data-stu-id="e9505-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="e9505-122">Você só pode filtrar por **displayName** ou **categorias.**</span><span class="sxs-lookup"><span data-stu-id="e9505-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="e9505-123">Por exemplo,  `$filter=contains(displayName, 'salesf')` ou `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="e9505-123">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="e9505-124">Você pode usar `$orderby` e `$top,` consultar `$skip` parâmetros em qualquer solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="e9505-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="e9505-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e9505-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9505-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9505-126">Request headers</span></span>

| <span data-ttu-id="e9505-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e9505-127">Name</span></span>      |<span data-ttu-id="e9505-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9505-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9505-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9505-129">Authorization</span></span> | <span data-ttu-id="e9505-130">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e9505-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9505-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9505-131">Request body</span></span>

<span data-ttu-id="e9505-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9505-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9505-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9505-133">Response</span></span>

<span data-ttu-id="e9505-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos applicationTemplate](../resources/applicationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9505-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9505-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9505-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9505-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9505-136">Request</span></span>

<span data-ttu-id="e9505-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9505-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9505-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9505-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="e9505-139">C#</span><span class="sxs-lookup"><span data-stu-id="e9505-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9505-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9505-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9505-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9505-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9505-142">Java</span><span class="sxs-lookup"><span data-stu-id="e9505-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9505-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9505-143">Response</span></span>

<span data-ttu-id="e9505-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9505-144">The following is an example of the response.</span></span>

> <span data-ttu-id="e9505-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e9505-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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



