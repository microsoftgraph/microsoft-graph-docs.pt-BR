---
title: Listar telefones
description: Recupere uma lista de objetos de isphone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 518e58f6bc516998d8609a3e51563eb09a70cfd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455135"
---
# <a name="list-phones"></a><span data-ttu-id="88cb7-103">Listar telefones</span><span class="sxs-lookup"><span data-stu-id="88cb7-103">List phones</span></span>

<span data-ttu-id="88cb7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="88cb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88cb7-105">Recupere uma lista de objetos de [Multiphone](../resources/itemphone.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="88cb7-105">Retrieve a list of [itemPhone](../resources/itemphone.md) objects from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="88cb7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88cb7-106">Permissions</span></span>

<span data-ttu-id="88cb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88cb7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88cb7-109">Permission type</span></span>                        | <span data-ttu-id="88cb7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88cb7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="88cb7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88cb7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="88cb7-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="88cb7-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="88cb7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88cb7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88cb7-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="88cb7-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="88cb7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88cb7-115">Application</span></span>                            | <span data-ttu-id="88cb7-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="88cb7-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="88cb7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88cb7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88cb7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88cb7-118">Optional query parameters</span></span>

<span data-ttu-id="88cb7-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88cb7-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="88cb7-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="88cb7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="88cb7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="88cb7-121">Name</span></span>            |<span data-ttu-id="88cb7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="88cb7-122">Value</span></span>    |<span data-ttu-id="88cb7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="88cb7-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="88cb7-124">$filter</span><span class="sxs-lookup"><span data-stu-id="88cb7-124">$filter</span></span>         |<span data-ttu-id="88cb7-125">string</span><span class="sxs-lookup"><span data-stu-id="88cb7-125">string</span></span>   |<span data-ttu-id="88cb7-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="88cb7-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="88cb7-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="88cb7-127">$orderby</span></span>        |<span data-ttu-id="88cb7-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88cb7-128">string</span></span>   |<span data-ttu-id="88cb7-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="88cb7-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="88cb7-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="88cb7-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="88cb7-131">$select</span><span class="sxs-lookup"><span data-stu-id="88cb7-131">$select</span></span>         |<span data-ttu-id="88cb7-132">string</span><span class="sxs-lookup"><span data-stu-id="88cb7-132">string</span></span>   |<span data-ttu-id="88cb7-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="88cb7-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="88cb7-135">$skip</span><span class="sxs-lookup"><span data-stu-id="88cb7-135">$skip</span></span>           |<span data-ttu-id="88cb7-136">int</span><span class="sxs-lookup"><span data-stu-id="88cb7-136">int</span></span>      |<span data-ttu-id="88cb7-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="88cb7-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="88cb7-138">$top</span><span class="sxs-lookup"><span data-stu-id="88cb7-138">$top</span></span>            |<span data-ttu-id="88cb7-139">int</span><span class="sxs-lookup"><span data-stu-id="88cb7-139">int</span></span>      |<span data-ttu-id="88cb7-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="88cb7-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="88cb7-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88cb7-141">Request headers</span></span>

| <span data-ttu-id="88cb7-142">Nome</span><span class="sxs-lookup"><span data-stu-id="88cb7-142">Name</span></span>           |<span data-ttu-id="88cb7-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="88cb7-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="88cb7-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="88cb7-144">Authorization</span></span>  | <span data-ttu-id="88cb7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88cb7-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="88cb7-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88cb7-147">Request body</span></span>

<span data-ttu-id="88cb7-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88cb7-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88cb7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="88cb7-149">Response</span></span>

<span data-ttu-id="88cb7-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [Tel](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88cb7-150">If successful, this method returns a `200 OK` response code and a collection of [itemPhone](../resources/itemphone.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88cb7-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="88cb7-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88cb7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88cb7-152">Request</span></span>

<span data-ttu-id="88cb7-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88cb7-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88cb7-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="88cb7-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phones"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/phones
```
# <a name="c"></a>[<span data-ttu-id="88cb7-155">C#</span><span class="sxs-lookup"><span data-stu-id="88cb7-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phones-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88cb7-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88cb7-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phones-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88cb7-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88cb7-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phones-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88cb7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="88cb7-158">Response</span></span>

<span data-ttu-id="88cb7-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88cb7-159">The following is an example of the response.</span></span>

> <span data-ttu-id="88cb7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88cb7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "type": "type-value",
      "number": "number-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List phones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
