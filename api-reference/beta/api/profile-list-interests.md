---
title: Listar interesses
description: Recupere uma lista de objetos personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 57337f9cb78cd06bbf3427864fb6131beafa1e66
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810742"
---
# <a name="list-interests"></a><span data-ttu-id="c17b7-103">Listar interesses</span><span class="sxs-lookup"><span data-stu-id="c17b7-103">List interests</span></span>

<span data-ttu-id="c17b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c17b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c17b7-105">Recupere uma lista de objetos [personInterest](../resources/personinterest.md) de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="c17b7-105">Retrieve a list of [personInterest](../resources/personinterest.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c17b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c17b7-106">Permissions</span></span>

<span data-ttu-id="c17b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c17b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c17b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c17b7-109">Permission type</span></span>                        | <span data-ttu-id="c17b7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c17b7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="c17b7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c17b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c17b7-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c17b7-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c17b7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c17b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c17b7-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c17b7-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c17b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c17b7-115">Application</span></span>                            | <span data-ttu-id="c17b7-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c17b7-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="c17b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c17b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests
GET /users/{id | userPrincipalName}/profile/interests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c17b7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c17b7-118">Optional query parameters</span></span>

<span data-ttu-id="c17b7-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c17b7-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="c17b7-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c17b7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="c17b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c17b7-121">Name</span></span>            |<span data-ttu-id="c17b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c17b7-122">Value</span></span>    |<span data-ttu-id="c17b7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c17b7-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="c17b7-124">$filter</span><span class="sxs-lookup"><span data-stu-id="c17b7-124">$filter</span></span>         |<span data-ttu-id="c17b7-125">string</span><span class="sxs-lookup"><span data-stu-id="c17b7-125">string</span></span>   |<span data-ttu-id="c17b7-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="c17b7-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="c17b7-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="c17b7-127">$orderby</span></span>        |<span data-ttu-id="c17b7-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c17b7-128">string</span></span>   |<span data-ttu-id="c17b7-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="c17b7-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="c17b7-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="c17b7-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="c17b7-131">$select</span><span class="sxs-lookup"><span data-stu-id="c17b7-131">$select</span></span>         |<span data-ttu-id="c17b7-132">string</span><span class="sxs-lookup"><span data-stu-id="c17b7-132">string</span></span>   |<span data-ttu-id="c17b7-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="c17b7-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="c17b7-135">$skip</span><span class="sxs-lookup"><span data-stu-id="c17b7-135">$skip</span></span>           |<span data-ttu-id="c17b7-136">int</span><span class="sxs-lookup"><span data-stu-id="c17b7-136">int</span></span>      |<span data-ttu-id="c17b7-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="c17b7-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="c17b7-138">$top</span><span class="sxs-lookup"><span data-stu-id="c17b7-138">$top</span></span>            |<span data-ttu-id="c17b7-139">int</span><span class="sxs-lookup"><span data-stu-id="c17b7-139">int</span></span>      |<span data-ttu-id="c17b7-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="c17b7-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="c17b7-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c17b7-141">Request headers</span></span>

| <span data-ttu-id="c17b7-142">Nome</span><span class="sxs-lookup"><span data-stu-id="c17b7-142">Name</span></span>           |<span data-ttu-id="c17b7-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c17b7-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="c17b7-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="c17b7-144">Authorization</span></span>  | <span data-ttu-id="c17b7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c17b7-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="c17b7-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c17b7-147">Request body</span></span>

<span data-ttu-id="c17b7-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c17b7-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c17b7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c17b7-149">Response</span></span>

<span data-ttu-id="c17b7-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [personInterest](../resources/personinterest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c17b7-150">If successful, this method returns a `200 OK` response code and a collection of [personInterest](../resources/personinterest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c17b7-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c17b7-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c17b7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c17b7-152">Request</span></span>

<span data-ttu-id="c17b7-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c17b7-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c17b7-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c17b7-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_interests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/interests
```
# <a name="c"></a>[<span data-ttu-id="c17b7-155">C#</span><span class="sxs-lookup"><span data-stu-id="c17b7-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c17b7-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c17b7-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c17b7-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c17b7-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c17b7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c17b7-158">Response</span></span>

<span data-ttu-id="c17b7-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c17b7-159">The following is an example of the response.</span></span>

> <span data-ttu-id="c17b7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c17b7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest",
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
      "categories": [
        "Sports"
      ],
      "description": "World's greatest football club",
      "displayName": "Chelsea FC",
      "webUrl": "https://www.chelseafc.com",
      "collaborationTags": null
    }
  ]
}
```
