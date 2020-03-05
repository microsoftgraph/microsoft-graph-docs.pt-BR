---
title: Obter personWebsite
description: Recupere as propriedades e os relacionamentos de um objeto personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 82ec32d364483df1406905d9457f8c8b79304503
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455851"
---
# <a name="get-personwebsite"></a><span data-ttu-id="a7b34-103">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="a7b34-103">Get personWebsite</span></span>

<span data-ttu-id="a7b34-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7b34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7b34-105">Recupere as propriedades e os relacionamentos de um objeto [personWebsite](../resources/personwebsite.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="a7b34-105">Retrieve the properties and relationships of a [personWebsite](../resources/personwebsite.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7b34-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7b34-106">Permissions</span></span>

<span data-ttu-id="a7b34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7b34-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7b34-109">Permission type</span></span>                        | <span data-ttu-id="a7b34-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7b34-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a7b34-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7b34-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7b34-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a7b34-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a7b34-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7b34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7b34-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a7b34-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a7b34-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7b34-115">Application</span></span>                            | <span data-ttu-id="a7b34-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a7b34-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="a7b34-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b34-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/websites/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7b34-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7b34-118">Optional query parameters</span></span>

<span data-ttu-id="a7b34-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7b34-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="a7b34-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a7b34-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="a7b34-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a7b34-121">Name</span></span>            |<span data-ttu-id="a7b34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7b34-122">Value</span></span>    |<span data-ttu-id="a7b34-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7b34-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="a7b34-124">$filter</span><span class="sxs-lookup"><span data-stu-id="a7b34-124">$filter</span></span>         |<span data-ttu-id="a7b34-125">string</span><span class="sxs-lookup"><span data-stu-id="a7b34-125">string</span></span>   |<span data-ttu-id="a7b34-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="a7b34-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="a7b34-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="a7b34-127">$orderby</span></span>        |<span data-ttu-id="a7b34-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7b34-128">string</span></span>   |<span data-ttu-id="a7b34-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="a7b34-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="a7b34-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="a7b34-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="a7b34-131">$select</span><span class="sxs-lookup"><span data-stu-id="a7b34-131">$select</span></span>         |<span data-ttu-id="a7b34-132">string</span><span class="sxs-lookup"><span data-stu-id="a7b34-132">string</span></span>   |<span data-ttu-id="a7b34-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="a7b34-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="a7b34-135">$skip</span><span class="sxs-lookup"><span data-stu-id="a7b34-135">$skip</span></span>           |<span data-ttu-id="a7b34-136">int</span><span class="sxs-lookup"><span data-stu-id="a7b34-136">int</span></span>      |<span data-ttu-id="a7b34-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="a7b34-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="a7b34-138">$top</span><span class="sxs-lookup"><span data-stu-id="a7b34-138">$top</span></span>            |<span data-ttu-id="a7b34-139">int</span><span class="sxs-lookup"><span data-stu-id="a7b34-139">int</span></span>      |<span data-ttu-id="a7b34-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a7b34-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="a7b34-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b34-141">Request headers</span></span>

| <span data-ttu-id="a7b34-142">Nome</span><span class="sxs-lookup"><span data-stu-id="a7b34-142">Name</span></span>           |<span data-ttu-id="a7b34-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7b34-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a7b34-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7b34-144">Authorization</span></span>  | <span data-ttu-id="a7b34-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7b34-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="a7b34-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b34-147">Request body</span></span>

<span data-ttu-id="a7b34-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7b34-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7b34-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b34-149">Response</span></span>

<span data-ttu-id="a7b34-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [personWebsite](../resources/personwebsite.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7b34-150">If successful, this method returns a `200 OK` response code and the requested [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7b34-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7b34-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7b34-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b34-152">Request</span></span>

<span data-ttu-id="a7b34-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7b34-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7b34-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b34-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personwebsite"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/websites/{id}
```
# <a name="c"></a>[<span data-ttu-id="a7b34-155">C#</span><span class="sxs-lookup"><span data-stu-id="a7b34-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7b34-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7b34-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7b34-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7b34-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7b34-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b34-158">Response</span></span>

<span data-ttu-id="a7b34-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7b34-159">The following is an example of the response.</span></span>

> <span data-ttu-id="a7b34-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7b34-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
