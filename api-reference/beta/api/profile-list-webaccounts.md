---
title: Listar contas da webaccount
description: Recupere uma lista de objetos webaccounts.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8363f4b831681f59b76d0ec0628dc7f9851501e6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978519"
---
# <a name="list-webaccounts"></a><span data-ttu-id="bca05-103">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="bca05-103">List webAccounts</span></span>

<span data-ttu-id="bca05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bca05-105">Recupere uma lista de objetos [Webaccounts](../resources/webaccount.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="bca05-105">Retrieve a list of [webAccounts](../resources/webaccount.md) objects from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bca05-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bca05-106">Permissions</span></span>

<span data-ttu-id="bca05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bca05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bca05-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bca05-109">Permission type</span></span>                        | <span data-ttu-id="bca05-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bca05-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="bca05-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bca05-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bca05-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bca05-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bca05-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bca05-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bca05-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bca05-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bca05-115">Application</span><span class="sxs-lookup"><span data-stu-id="bca05-115">Application</span></span>                            | <span data-ttu-id="bca05-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bca05-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="bca05-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bca05-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/webAccounts
GET /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bca05-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bca05-118">Optional query parameters</span></span>

<span data-ttu-id="bca05-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bca05-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="bca05-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bca05-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="bca05-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bca05-121">Name</span></span>            |<span data-ttu-id="bca05-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bca05-122">Value</span></span>    |<span data-ttu-id="bca05-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca05-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="bca05-124">$filter</span><span class="sxs-lookup"><span data-stu-id="bca05-124">$filter</span></span>         |<span data-ttu-id="bca05-125">string</span><span class="sxs-lookup"><span data-stu-id="bca05-125">string</span></span>   |<span data-ttu-id="bca05-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="bca05-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="bca05-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="bca05-127">$orderby</span></span>        |<span data-ttu-id="bca05-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bca05-128">string</span></span>   |<span data-ttu-id="bca05-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="bca05-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="bca05-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="bca05-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="bca05-131">$select</span><span class="sxs-lookup"><span data-stu-id="bca05-131">$select</span></span>         |<span data-ttu-id="bca05-132">string</span><span class="sxs-lookup"><span data-stu-id="bca05-132">string</span></span>   |<span data-ttu-id="bca05-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="bca05-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="bca05-135">$skip</span><span class="sxs-lookup"><span data-stu-id="bca05-135">$skip</span></span>           |<span data-ttu-id="bca05-136">int</span><span class="sxs-lookup"><span data-stu-id="bca05-136">int</span></span>      |<span data-ttu-id="bca05-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="bca05-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="bca05-138">$top</span><span class="sxs-lookup"><span data-stu-id="bca05-138">$top</span></span>            |<span data-ttu-id="bca05-139">int</span><span class="sxs-lookup"><span data-stu-id="bca05-139">int</span></span>      |<span data-ttu-id="bca05-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="bca05-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="bca05-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bca05-141">Request headers</span></span>

| <span data-ttu-id="bca05-142">Nome</span><span class="sxs-lookup"><span data-stu-id="bca05-142">Name</span></span>           |<span data-ttu-id="bca05-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca05-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bca05-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="bca05-144">Authorization</span></span>  | <span data-ttu-id="bca05-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bca05-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="bca05-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bca05-147">Request body</span></span>

<span data-ttu-id="bca05-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bca05-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bca05-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="bca05-149">Response</span></span>

<span data-ttu-id="bca05-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [webaccount](../resources/webaccount.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bca05-150">If successful, this method returns a `200 OK` response code and a collection of [webAccount](../resources/webaccount.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bca05-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bca05-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bca05-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bca05-152">Request</span></span>

<span data-ttu-id="bca05-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bca05-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bca05-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="bca05-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_webaccounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/webAccounts
```
# <a name="c"></a>[<span data-ttu-id="bca05-155">C#</span><span class="sxs-lookup"><span data-stu-id="bca05-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-webaccounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bca05-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bca05-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-webaccounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bca05-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bca05-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-webaccounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bca05-158">Java</span><span class="sxs-lookup"><span data-stu-id="bca05-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-webaccounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bca05-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bca05-159">Response</span></span>

<span data-ttu-id="bca05-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bca05-160">The following is an example of the response.</span></span>

> <span data-ttu-id="bca05-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bca05-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "source": null,
      "description": "My Github contributions!",
      "userId": "innocenty.popov",
      "service": {
        "name": "GitHub",
        "webUrl": "https://github.com"
      },
      "statusMessage": null,
      "webUrl": "https://github.com/innocenty.popov"
    }
  ]
}
```


