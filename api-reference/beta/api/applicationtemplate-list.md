---
title: Listar applicationTemplates
description: Recupere uma lista de objetos applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d74e274d2db8d20cb9cf3269ab78cc12055b76c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439515"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="b0c9e-103">Listar applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="b0c9e-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c9e-104">Recupere uma lista de [](../resources/applicationtemplate.md) objetos applicationtemplate da Galeria de aplicativos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0c9e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0c9e-105">Permissions</span></span>

<span data-ttu-id="b0c9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0c9e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0c9e-108">Permission type</span></span>                        | <span data-ttu-id="b0c9e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0c9e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0c9e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0c9e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0c9e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-111">None.</span></span> |
| <span data-ttu-id="b0c9e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0c9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0c9e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-113">Not supported.</span></span> |
| <span data-ttu-id="b0c9e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0c9e-114">Application</span></span>                            | <span data-ttu-id="b0c9e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-115">None.</span></span> |

<span data-ttu-id="b0c9e-116">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="b0c9e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0c9e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0c9e-118">Optional query parameters</span></span>

<span data-ttu-id="b0c9e-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="b0c9e-120">Você pode usar o `$filter` parâmetro de forma limitada.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="b0c9e-121">Você só pode filtrar por **DisplayName** ou **categorias**.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="b0c9e-122">Por exemplo,  `$filter=contains(displayName, 'salesf')` ou `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="b0c9e-123">Você pode usar `$orderby` `$top,` e `$skip` consultar parâmetros em qualquer solicitação get.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="b0c9e-124">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b0c9e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0c9e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c9e-125">Request headers</span></span>

| <span data-ttu-id="b0c9e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b0c9e-126">Name</span></span>      |<span data-ttu-id="b0c9e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c9e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0c9e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0c9e-128">Authorization</span></span> | <span data-ttu-id="b0c9e-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b0c9e-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0c9e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c9e-130">Request body</span></span>

<span data-ttu-id="b0c9e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0c9e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0c9e-132">Response</span></span>

<span data-ttu-id="b0c9e-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [applicationtemplate](../resources/applicationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0c9e-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b0c9e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0c9e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c9e-135">Request</span></span>

<span data-ttu-id="b0c9e-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0c9e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c9e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0c9e-138">C#</span><span class="sxs-lookup"><span data-stu-id="b0c9e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0c9e-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0c9e-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0c9e-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b0c9e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0c9e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0c9e-141">Response</span></span>

<span data-ttu-id="b0c9e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b0c9e-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b0c9e-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0c9e-144">All the properties will be returned from an actual call.</span></span>

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
