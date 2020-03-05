---
title: Listar contas da webaccount
description: Recupere uma lista de objetos webaccounts.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 75d45c0dff4828c292887e7d7fb1d8a6817c53dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455150"
---
# <a name="list-webaccounts"></a><span data-ttu-id="d2f28-103">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="d2f28-103">List webAccounts</span></span>

<span data-ttu-id="d2f28-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2f28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f28-105">Recupere uma lista de objetos [Webaccounts](../resources/webaccount.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2f28-105">Retrieve a list of [webAccounts](../resources/webaccount.md) objects from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f28-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2f28-106">Permissions</span></span>

<span data-ttu-id="d2f28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2f28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2f28-109">Permission type</span></span>                        | <span data-ttu-id="d2f28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2f28-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d2f28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2f28-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2f28-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2f28-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d2f28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2f28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f28-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2f28-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d2f28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2f28-115">Application</span></span>                            | <span data-ttu-id="d2f28-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2f28-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d2f28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2f28-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/webAccounts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2f28-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2f28-118">Optional query parameters</span></span>

<span data-ttu-id="d2f28-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2f28-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="d2f28-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d2f28-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="d2f28-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d2f28-121">Name</span></span>            |<span data-ttu-id="d2f28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d2f28-122">Value</span></span>    |<span data-ttu-id="d2f28-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2f28-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d2f28-124">$filter</span><span class="sxs-lookup"><span data-stu-id="d2f28-124">$filter</span></span>         |<span data-ttu-id="d2f28-125">string</span><span class="sxs-lookup"><span data-stu-id="d2f28-125">string</span></span>   |<span data-ttu-id="d2f28-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="d2f28-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="d2f28-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="d2f28-127">$orderby</span></span>        |<span data-ttu-id="d2f28-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2f28-128">string</span></span>   |<span data-ttu-id="d2f28-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="d2f28-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="d2f28-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="d2f28-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="d2f28-131">$select</span><span class="sxs-lookup"><span data-stu-id="d2f28-131">$select</span></span>         |<span data-ttu-id="d2f28-132">string</span><span class="sxs-lookup"><span data-stu-id="d2f28-132">string</span></span>   |<span data-ttu-id="d2f28-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="d2f28-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="d2f28-135">$skip</span><span class="sxs-lookup"><span data-stu-id="d2f28-135">$skip</span></span>           |<span data-ttu-id="d2f28-136">int</span><span class="sxs-lookup"><span data-stu-id="d2f28-136">int</span></span>      |<span data-ttu-id="d2f28-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="d2f28-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="d2f28-138">$top</span><span class="sxs-lookup"><span data-stu-id="d2f28-138">$top</span></span>            |<span data-ttu-id="d2f28-139">int</span><span class="sxs-lookup"><span data-stu-id="d2f28-139">int</span></span>      |<span data-ttu-id="d2f28-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="d2f28-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="d2f28-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2f28-141">Request headers</span></span>

| <span data-ttu-id="d2f28-142">Nome</span><span class="sxs-lookup"><span data-stu-id="d2f28-142">Name</span></span>           |<span data-ttu-id="d2f28-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2f28-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d2f28-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2f28-144">Authorization</span></span>  | <span data-ttu-id="d2f28-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2f28-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="d2f28-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2f28-147">Request body</span></span>

<span data-ttu-id="d2f28-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2f28-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2f28-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2f28-149">Response</span></span>

<span data-ttu-id="d2f28-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [webaccount](../resources/webaccount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2f28-150">If successful, this method returns a `200 OK` response code and a collection of [webAccount](../resources/webaccount.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2f28-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2f28-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2f28-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2f28-152">Request</span></span>

<span data-ttu-id="d2f28-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2f28-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2f28-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2f28-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_webaccounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/webAccounts
```
# <a name="c"></a>[<span data-ttu-id="d2f28-155">C#</span><span class="sxs-lookup"><span data-stu-id="d2f28-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-webaccounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2f28-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2f28-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-webaccounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2f28-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2f28-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-webaccounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2f28-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2f28-158">Response</span></span>

<span data-ttu-id="d2f28-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2f28-159">The following is an example of the response.</span></span>

> <span data-ttu-id="d2f28-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2f28-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "userId": "userId-value",
      "service": {
        "name": "name-value",
        "webUrl": "webUrl-value"
      },
      "statusMessage": "statusMessage-value",
      "webUrl": "webUrl-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List webAccounts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
