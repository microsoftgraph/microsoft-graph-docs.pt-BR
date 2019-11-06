---
title: Listar conta
description: Recupere uma lista de objetos useraccountinformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 800814e1b8d342e4d0d118101dccf65007250514
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998012"
---
# <a name="list-account"></a><span data-ttu-id="6d052-103">Listar conta</span><span class="sxs-lookup"><span data-stu-id="6d052-103">List account</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d052-104">Recupera as propriedades relacionadas à conta do usuário do [perfil](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="6d052-104">Retrieves properties related to the user's account from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d052-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d052-105">Permissions</span></span>

<span data-ttu-id="6d052-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d052-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d052-108">Permission type</span></span>                        | <span data-ttu-id="6d052-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d052-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6d052-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d052-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d052-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d052-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6d052-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d052-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d052-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d052-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6d052-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d052-114">Application</span></span>                            | <span data-ttu-id="6d052-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6d052-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="6d052-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d052-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d052-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d052-117">Optional query parameters</span></span>

<span data-ttu-id="6d052-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d052-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="6d052-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6d052-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="6d052-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6d052-120">Name</span></span>            |<span data-ttu-id="6d052-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d052-121">Value</span></span>    |<span data-ttu-id="6d052-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d052-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6d052-123">$filter</span><span class="sxs-lookup"><span data-stu-id="6d052-123">$filter</span></span>         |<span data-ttu-id="6d052-124">string</span><span class="sxs-lookup"><span data-stu-id="6d052-124">string</span></span>   |<span data-ttu-id="6d052-125">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="6d052-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="6d052-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="6d052-126">$orderby</span></span>        |<span data-ttu-id="6d052-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d052-127">string</span></span>   |<span data-ttu-id="6d052-128">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="6d052-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="6d052-129">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="6d052-129">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="6d052-130">$select</span><span class="sxs-lookup"><span data-stu-id="6d052-130">$select</span></span>         |<span data-ttu-id="6d052-131">string</span><span class="sxs-lookup"><span data-stu-id="6d052-131">string</span></span>   |<span data-ttu-id="6d052-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="6d052-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="6d052-134">$skip</span><span class="sxs-lookup"><span data-stu-id="6d052-134">$skip</span></span>           |<span data-ttu-id="6d052-135">int</span><span class="sxs-lookup"><span data-stu-id="6d052-135">int</span></span>      |<span data-ttu-id="6d052-136">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="6d052-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="6d052-137">$top</span><span class="sxs-lookup"><span data-stu-id="6d052-137">$top</span></span>            |<span data-ttu-id="6d052-138">int</span><span class="sxs-lookup"><span data-stu-id="6d052-138">int</span></span>      |<span data-ttu-id="6d052-139">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="6d052-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="6d052-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d052-140">Request headers</span></span>

| <span data-ttu-id="6d052-141">Nome</span><span class="sxs-lookup"><span data-stu-id="6d052-141">Name</span></span>           |<span data-ttu-id="6d052-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d052-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6d052-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d052-143">Authorization</span></span>  | <span data-ttu-id="6d052-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d052-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6d052-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d052-146">Content-Type</span></span>   | <span data-ttu-id="6d052-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d052-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d052-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d052-149">Request body</span></span>

<span data-ttu-id="6d052-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d052-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d052-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d052-151">Response</span></span>

<span data-ttu-id="6d052-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d052-152">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d052-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6d052-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d052-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d052-154">Request</span></span>

<span data-ttu-id="6d052-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d052-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d052-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d052-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d052-157">C#</span><span class="sxs-lookup"><span data-stu-id="6d052-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-account-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d052-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d052-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-account-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d052-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d052-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-account-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d052-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d052-160">Response</span></span>

<span data-ttu-id="6d052-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d052-161">The following is an example of the response.</span></span>

> <span data-ttu-id="6d052-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d052-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "ageGroup": "ageGroup-value",
      "countryCode": "countryCode-value",
      "preferredLanguageTag": {
        "locale": "locale-value",
        "displayName": "displayName-value"
      },
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List account",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
