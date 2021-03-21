---
title: Listar nomes
description: Recupere uma lista de objetos personName do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a6d3dadfb3b8565519adf7fc1c95ee593bb57d83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957195"
---
# <a name="list-names"></a><span data-ttu-id="026e0-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="026e0-103">List names</span></span>

<span data-ttu-id="026e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="026e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="026e0-105">Recupere uma lista de [objetos personName](../resources/personname.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="026e0-105">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="026e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="026e0-106">Permissions</span></span>

<span data-ttu-id="026e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="026e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="026e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="026e0-109">Permission type</span></span>                        | <span data-ttu-id="026e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="026e0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="026e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="026e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="026e0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026e0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="026e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="026e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="026e0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026e0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="026e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="026e0-115">Application</span></span>                            | <span data-ttu-id="026e0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026e0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="026e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="026e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
GET /users/{id | userPrincipalName}/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="026e0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="026e0-118">Optional query parameters</span></span>

<span data-ttu-id="026e0-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="026e0-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="026e0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="026e0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="026e0-121">Name</span><span class="sxs-lookup"><span data-stu-id="026e0-121">Name</span></span>            |<span data-ttu-id="026e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="026e0-122">Value</span></span>    |<span data-ttu-id="026e0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="026e0-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="026e0-124">$filter</span><span class="sxs-lookup"><span data-stu-id="026e0-124">$filter</span></span>         |<span data-ttu-id="026e0-125">string</span><span class="sxs-lookup"><span data-stu-id="026e0-125">string</span></span>   |<span data-ttu-id="026e0-126">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="026e0-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="026e0-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="026e0-127">$orderby</span></span>        |<span data-ttu-id="026e0-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="026e0-128">string</span></span>   |<span data-ttu-id="026e0-129">Por padrão, os objetos na resposta são classificação pelo valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="026e0-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="026e0-130">Você pode alterar a ordem da resposta usando o parâmetro *$orderby.*</span><span class="sxs-lookup"><span data-stu-id="026e0-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="026e0-131">$select</span><span class="sxs-lookup"><span data-stu-id="026e0-131">$select</span></span>         |<span data-ttu-id="026e0-132">string</span><span class="sxs-lookup"><span data-stu-id="026e0-132">string</span></span>   |<span data-ttu-id="026e0-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="026e0-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="026e0-135">$skip</span><span class="sxs-lookup"><span data-stu-id="026e0-135">$skip</span></span>           |<span data-ttu-id="026e0-136">int</span><span class="sxs-lookup"><span data-stu-id="026e0-136">int</span></span>      |<span data-ttu-id="026e0-137">Ignore os primeiros resultados n, úteis para pajamento.</span><span class="sxs-lookup"><span data-stu-id="026e0-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="026e0-138">$top</span><span class="sxs-lookup"><span data-stu-id="026e0-138">$top</span></span>            |<span data-ttu-id="026e0-139">int</span><span class="sxs-lookup"><span data-stu-id="026e0-139">int</span></span>      |<span data-ttu-id="026e0-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="026e0-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="026e0-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="026e0-141">Request headers</span></span>

| <span data-ttu-id="026e0-142">Nome</span><span class="sxs-lookup"><span data-stu-id="026e0-142">Name</span></span>           |<span data-ttu-id="026e0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="026e0-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="026e0-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="026e0-144">Authorization</span></span>  | <span data-ttu-id="026e0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="026e0-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="026e0-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="026e0-147">Content-Type</span></span>   | <span data-ttu-id="026e0-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="026e0-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="026e0-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="026e0-150">Request body</span></span>

<span data-ttu-id="026e0-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="026e0-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="026e0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="026e0-152">Response</span></span>

<span data-ttu-id="026e0-153">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos personName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="026e0-153">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="026e0-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="026e0-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="026e0-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="026e0-155">Request</span></span>

<span data-ttu-id="026e0-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="026e0-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="026e0-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="026e0-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names
```
# <a name="c"></a>[<span data-ttu-id="026e0-158">C#</span><span class="sxs-lookup"><span data-stu-id="026e0-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="026e0-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="026e0-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="026e0-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="026e0-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="026e0-161">Java</span><span class="sxs-lookup"><span data-stu-id="026e0-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-names-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="026e0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="026e0-162">Response</span></span>

<span data-ttu-id="026e0-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="026e0-163">The following is an example of the response.</span></span>

> <span data-ttu-id="026e0-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="026e0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
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
      "displayName": "Innocenty Popov",
      "first": "Innocenty",
      "initials": "IP",
      "last": "Popov",
      "languageTag": "en-US",
      "maiden": null,
      "middle": null,
      "nickname": "Kesha",
      "suffix": null,
      "title": null,
      "pronunciation": {
        "displayName": "In-no ken-te ",
        "first": "In-no ken-te Pop-ov",
        "maiden": null,
        "middle": null,
        "last": "Pop-ov"
      }
    }
  ]
}
```


