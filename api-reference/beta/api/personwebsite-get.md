---
title: Obter personWebsite
description: Recupere as propriedades e os relacionamentos de um objeto personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9c12cdc0547bddeb2ee505b01aee39d96be41441
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228685"
---
# <a name="get-personwebsite"></a><span data-ttu-id="e1449-103">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="e1449-103">Get personWebsite</span></span>

<span data-ttu-id="e1449-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1449-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1449-105">Recupere as propriedades e os relacionamentos de um objeto [personWebsite](../resources/personwebsite.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="e1449-105">Retrieve the properties and relationships of a [personWebsite](../resources/personwebsite.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1449-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1449-106">Permissions</span></span>

<span data-ttu-id="e1449-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1449-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1449-109">Permission type</span></span>                        | <span data-ttu-id="e1449-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1449-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e1449-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1449-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1449-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1449-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e1449-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1449-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1449-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1449-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e1449-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1449-115">Application</span></span>                            | <span data-ttu-id="e1449-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1449-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e1449-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1449-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/websites/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1449-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1449-118">Optional query parameters</span></span>

<span data-ttu-id="e1449-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1449-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="e1449-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e1449-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="e1449-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e1449-121">Name</span></span>            |<span data-ttu-id="e1449-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1449-122">Value</span></span>    |<span data-ttu-id="e1449-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1449-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e1449-124">$filter</span><span class="sxs-lookup"><span data-stu-id="e1449-124">$filter</span></span>         |<span data-ttu-id="e1449-125">string</span><span class="sxs-lookup"><span data-stu-id="e1449-125">string</span></span>   |<span data-ttu-id="e1449-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="e1449-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="e1449-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="e1449-127">$orderby</span></span>        |<span data-ttu-id="e1449-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1449-128">string</span></span>   |<span data-ttu-id="e1449-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="e1449-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="e1449-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="e1449-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="e1449-131">$select</span><span class="sxs-lookup"><span data-stu-id="e1449-131">$select</span></span>         |<span data-ttu-id="e1449-132">string</span><span class="sxs-lookup"><span data-stu-id="e1449-132">string</span></span>   |<span data-ttu-id="e1449-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="e1449-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="e1449-135">$skip</span><span class="sxs-lookup"><span data-stu-id="e1449-135">$skip</span></span>           |<span data-ttu-id="e1449-136">int</span><span class="sxs-lookup"><span data-stu-id="e1449-136">int</span></span>      |<span data-ttu-id="e1449-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="e1449-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="e1449-138">$top</span><span class="sxs-lookup"><span data-stu-id="e1449-138">$top</span></span>            |<span data-ttu-id="e1449-139">int</span><span class="sxs-lookup"><span data-stu-id="e1449-139">int</span></span>      |<span data-ttu-id="e1449-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="e1449-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="e1449-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1449-141">Request headers</span></span>

| <span data-ttu-id="e1449-142">Nome</span><span class="sxs-lookup"><span data-stu-id="e1449-142">Name</span></span>           |<span data-ttu-id="e1449-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1449-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e1449-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1449-144">Authorization</span></span>  | <span data-ttu-id="e1449-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1449-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="e1449-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1449-147">Request body</span></span>

<span data-ttu-id="e1449-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1449-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1449-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1449-149">Response</span></span>

<span data-ttu-id="e1449-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [personWebsite](../resources/personwebsite.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1449-150">If successful, this method returns a `200 OK` response code and the requested [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1449-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e1449-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1449-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1449-152">Request</span></span>

<span data-ttu-id="e1449-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1449-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1449-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1449-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personwebsite"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/websites/{id}
```
# <a name="c"></a>[<span data-ttu-id="e1449-155">C#</span><span class="sxs-lookup"><span data-stu-id="e1449-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1449-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1449-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1449-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1449-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e1449-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1449-158">Response</span></span>

<span data-ttu-id="e1449-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1449-159">The following is an example of the response.</span></span>

> <span data-ttu-id="e1449-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1449-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get personWebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
