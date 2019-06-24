---
title: Listar applicationTemplates
description: Recupere uma lista de objetos applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac8ad3a8b4a7a396c0cb35c1c72c2d1a2e309184
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147883"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="1d2f4-103">Listar applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="1d2f4-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d2f4-104">Recupere uma lista de [](../resources/applicationtemplate.md) objetos applicationtemplate da Galeria de aplicativos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d2f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d2f4-105">Permissions</span></span>

<span data-ttu-id="1d2f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d2f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d2f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d2f4-108">Permission type</span></span>                        | <span data-ttu-id="1d2f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d2f4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1d2f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d2f4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d2f4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-111">None.</span></span> |
| <span data-ttu-id="1d2f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d2f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d2f4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-113">Not supported.</span></span> |
| <span data-ttu-id="1d2f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d2f4-114">Application</span></span>                            | <span data-ttu-id="1d2f4-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-115">None.</span></span> |

<span data-ttu-id="1d2f4-116">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d2f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d2f4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d2f4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d2f4-118">Optional query parameters</span></span>

<span data-ttu-id="1d2f4-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="1d2f4-120">Você pode usar o `$filter` parâmetro de forma limitada.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="1d2f4-121">Você só pode filtrar por **DisplayName** ou **categorias**.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="1d2f4-122">Por exemplo,  `$filter=contains(displayName, 'salesf')` ou `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="1d2f4-123">Você pode usar `$orderby` `$top,` e `$skip` consultar parâmetros em qualquer solicitação get.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="1d2f4-124">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1d2f4-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d2f4-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2f4-125">Request headers</span></span>

| <span data-ttu-id="1d2f4-126">Nome</span><span class="sxs-lookup"><span data-stu-id="1d2f4-126">Name</span></span>      |<span data-ttu-id="1d2f4-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d2f4-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d2f4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d2f4-128">Authorization</span></span> | <span data-ttu-id="1d2f4-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1d2f4-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d2f4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2f4-130">Request body</span></span>

<span data-ttu-id="1d2f4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d2f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2f4-132">Response</span></span>

<span data-ttu-id="1d2f4-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [applicationtemplate](../resources/applicationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d2f4-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d2f4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d2f4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2f4-135">Request</span></span>

<span data-ttu-id="1d2f4-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```

### <a name="response"></a><span data-ttu-id="1d2f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2f4-137">Response</span></span>

<span data-ttu-id="1d2f4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1d2f4-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1d2f4-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d2f4-140">All the properties will be returned from an actual call.</span></span>

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
