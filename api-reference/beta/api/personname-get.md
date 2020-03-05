---
title: Obter PersonName
description: Recupere as propriedades e os relacionamentos de um objeto PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8258abf0b39163ecce62ac601f52f8cbcec42004
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455885"
---
# <a name="get-personname"></a><span data-ttu-id="f1dcd-103">Obter PersonName</span><span class="sxs-lookup"><span data-stu-id="f1dcd-103">Get personName</span></span>

<span data-ttu-id="f1dcd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1dcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1dcd-105">Recupere as propriedades e os relacionamentos de um objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-105">Retrieve the properties and relationships of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1dcd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1dcd-106">Permissions</span></span>

<span data-ttu-id="f1dcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1dcd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1dcd-109">Permission type</span></span>                        | <span data-ttu-id="f1dcd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1dcd-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f1dcd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1dcd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1dcd-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1dcd-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f1dcd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1dcd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1dcd-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1dcd-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f1dcd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1dcd-115">Application</span></span>                            | <span data-ttu-id="f1dcd-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1dcd-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f1dcd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1dcd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1dcd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1dcd-118">Optional query parameters</span></span>

<span data-ttu-id="f1dcd-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="f1dcd-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f1dcd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="f1dcd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f1dcd-121">Name</span></span>            |<span data-ttu-id="f1dcd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1dcd-122">Value</span></span>    |<span data-ttu-id="f1dcd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1dcd-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f1dcd-124">$filter</span><span class="sxs-lookup"><span data-stu-id="f1dcd-124">$filter</span></span>         |<span data-ttu-id="f1dcd-125">string</span><span class="sxs-lookup"><span data-stu-id="f1dcd-125">string</span></span>   |<span data-ttu-id="f1dcd-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="f1dcd-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="f1dcd-127">$orderby</span></span>        |<span data-ttu-id="f1dcd-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1dcd-128">string</span></span>   |<span data-ttu-id="f1dcd-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="f1dcd-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="f1dcd-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="f1dcd-131">$select</span><span class="sxs-lookup"><span data-stu-id="f1dcd-131">$select</span></span>         |<span data-ttu-id="f1dcd-132">string</span><span class="sxs-lookup"><span data-stu-id="f1dcd-132">string</span></span>   |<span data-ttu-id="f1dcd-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="f1dcd-135">$skip</span><span class="sxs-lookup"><span data-stu-id="f1dcd-135">$skip</span></span>           |<span data-ttu-id="f1dcd-136">int</span><span class="sxs-lookup"><span data-stu-id="f1dcd-136">int</span></span>      |<span data-ttu-id="f1dcd-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="f1dcd-138">$top</span><span class="sxs-lookup"><span data-stu-id="f1dcd-138">$top</span></span>            |<span data-ttu-id="f1dcd-139">int</span><span class="sxs-lookup"><span data-stu-id="f1dcd-139">int</span></span>      |<span data-ttu-id="f1dcd-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="f1dcd-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1dcd-141">Request headers</span></span>

| <span data-ttu-id="f1dcd-142">Nome</span><span class="sxs-lookup"><span data-stu-id="f1dcd-142">Name</span></span>           |<span data-ttu-id="f1dcd-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1dcd-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f1dcd-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1dcd-144">Authorization</span></span>  | <span data-ttu-id="f1dcd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f1dcd-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1dcd-147">Content-Type</span></span>   | <span data-ttu-id="f1dcd-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1dcd-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1dcd-150">Request body</span></span>

<span data-ttu-id="f1dcd-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1dcd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1dcd-152">Response</span></span>

<span data-ttu-id="f1dcd-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [PersonName](../resources/personname.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-153">If successful, this method returns a `200 OK` response code and the requested [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1dcd-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1dcd-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1dcd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1dcd-155">Request</span></span>

<span data-ttu-id="f1dcd-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1dcd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1dcd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personname"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="c"></a>[<span data-ttu-id="f1dcd-158">C#</span><span class="sxs-lookup"><span data-stu-id="f1dcd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1dcd-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1dcd-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1dcd-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1dcd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1dcd-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1dcd-161">Response</span></span>

<span data-ttu-id="f1dcd-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-162">The following is an example of the response.</span></span>

> <span data-ttu-id="f1dcd-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1dcd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
