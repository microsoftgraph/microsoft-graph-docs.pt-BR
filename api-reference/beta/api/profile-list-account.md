---
title: Listar contas
description: Recupere uma lista de objetos userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fa7f1be3e871461d098544c3b29156e707f6f389
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229357"
---
# <a name="list-accounts"></a><span data-ttu-id="7eb1a-103">Listar contas</span><span class="sxs-lookup"><span data-stu-id="7eb1a-103">List accounts</span></span>

<span data-ttu-id="7eb1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eb1a-105">Recupera as propriedades relacionadas às contas do usuário a partir do [perfil](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-105">Retrieves properties related to the user's accounts from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7eb1a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7eb1a-106">Permissions</span></span>

<span data-ttu-id="7eb1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7eb1a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7eb1a-109">Permission type</span></span>                        | <span data-ttu-id="7eb1a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7eb1a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="7eb1a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7eb1a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7eb1a-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7eb1a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7eb1a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7eb1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eb1a-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7eb1a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7eb1a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7eb1a-115">Application</span></span>                            | <span data-ttu-id="7eb1a-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7eb1a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="7eb1a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb1a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7eb1a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7eb1a-118">Optional query parameters</span></span>

<span data-ttu-id="7eb1a-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="7eb1a-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7eb1a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="7eb1a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7eb1a-121">Name</span></span>            |<span data-ttu-id="7eb1a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7eb1a-122">Value</span></span>    |<span data-ttu-id="7eb1a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb1a-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7eb1a-124">$filter</span><span class="sxs-lookup"><span data-stu-id="7eb1a-124">$filter</span></span>         |<span data-ttu-id="7eb1a-125">string</span><span class="sxs-lookup"><span data-stu-id="7eb1a-125">string</span></span>   |<span data-ttu-id="7eb1a-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="7eb1a-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="7eb1a-127">$orderby</span></span>        |<span data-ttu-id="7eb1a-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7eb1a-128">string</span></span>   |<span data-ttu-id="7eb1a-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="7eb1a-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="7eb1a-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="7eb1a-131">$select</span><span class="sxs-lookup"><span data-stu-id="7eb1a-131">$select</span></span>         |<span data-ttu-id="7eb1a-132">string</span><span class="sxs-lookup"><span data-stu-id="7eb1a-132">string</span></span>   |<span data-ttu-id="7eb1a-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="7eb1a-135">$skip</span><span class="sxs-lookup"><span data-stu-id="7eb1a-135">$skip</span></span>           |<span data-ttu-id="7eb1a-136">int</span><span class="sxs-lookup"><span data-stu-id="7eb1a-136">int</span></span>      |<span data-ttu-id="7eb1a-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="7eb1a-138">$top</span><span class="sxs-lookup"><span data-stu-id="7eb1a-138">$top</span></span>            |<span data-ttu-id="7eb1a-139">int</span><span class="sxs-lookup"><span data-stu-id="7eb1a-139">int</span></span>      |<span data-ttu-id="7eb1a-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="7eb1a-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb1a-141">Request headers</span></span>

| <span data-ttu-id="7eb1a-142">Nome</span><span class="sxs-lookup"><span data-stu-id="7eb1a-142">Name</span></span>           |<span data-ttu-id="7eb1a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb1a-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7eb1a-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="7eb1a-144">Authorization</span></span>  | <span data-ttu-id="7eb1a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7eb1a-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7eb1a-147">Content-Type</span></span>   | <span data-ttu-id="7eb1a-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7eb1a-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb1a-150">Request body</span></span>

<span data-ttu-id="7eb1a-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eb1a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb1a-152">Response</span></span>

<span data-ttu-id="7eb1a-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-153">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7eb1a-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7eb1a-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7eb1a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb1a-155">Request</span></span>

<span data-ttu-id="7eb1a-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7eb1a-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb1a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```
# <a name="c"></a>[<span data-ttu-id="7eb1a-158">C#</span><span class="sxs-lookup"><span data-stu-id="7eb1a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-account-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7eb1a-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7eb1a-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-account-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7eb1a-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7eb1a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-account-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7eb1a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb1a-161">Response</span></span>

<span data-ttu-id="7eb1a-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-162">The following is an example of the response.</span></span>

> <span data-ttu-id="7eb1a-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7eb1a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
