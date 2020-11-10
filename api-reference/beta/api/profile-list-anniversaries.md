---
title: Listar aniversários
description: Recupere uma lista de objetos personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5e6ff2780ac62396f9df573ff8405befb0083180
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970188"
---
# <a name="list-anniversaries"></a><span data-ttu-id="f5592-103">Listar aniversários</span><span class="sxs-lookup"><span data-stu-id="f5592-103">List anniversaries</span></span>

<span data-ttu-id="f5592-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5592-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5592-105">Recupere uma lista de objetos [personAnniversary](../resources/personanniversary.md) para o usuário específico do seu [perfil](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="f5592-105">Retrieve a list of [personAnniversary](../resources/personanniversary.md) objects for the given user from their [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5592-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5592-106">Permissions</span></span>

<span data-ttu-id="f5592-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5592-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5592-109">Permission type</span></span>                        | <span data-ttu-id="f5592-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5592-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f5592-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5592-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5592-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f5592-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f5592-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5592-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5592-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f5592-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f5592-115">Application</span><span class="sxs-lookup"><span data-stu-id="f5592-115">Application</span></span>                            | <span data-ttu-id="f5592-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f5592-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f5592-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5592-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/anniversaries
GET /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5592-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5592-118">Optional query parameters</span></span>

<span data-ttu-id="f5592-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5592-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="f5592-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f5592-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="f5592-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f5592-121">Name</span></span>            |<span data-ttu-id="f5592-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5592-122">Value</span></span>    |<span data-ttu-id="f5592-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5592-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f5592-124">$filter</span><span class="sxs-lookup"><span data-stu-id="f5592-124">$filter</span></span>         |<span data-ttu-id="f5592-125">string</span><span class="sxs-lookup"><span data-stu-id="f5592-125">string</span></span>   |<span data-ttu-id="f5592-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="f5592-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="f5592-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="f5592-127">$orderby</span></span>        |<span data-ttu-id="f5592-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5592-128">string</span></span>   |<span data-ttu-id="f5592-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="f5592-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="f5592-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="f5592-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="f5592-131">$select</span><span class="sxs-lookup"><span data-stu-id="f5592-131">$select</span></span>         |<span data-ttu-id="f5592-132">string</span><span class="sxs-lookup"><span data-stu-id="f5592-132">string</span></span>   |<span data-ttu-id="f5592-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="f5592-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="f5592-135">$skip</span><span class="sxs-lookup"><span data-stu-id="f5592-135">$skip</span></span>           |<span data-ttu-id="f5592-136">int</span><span class="sxs-lookup"><span data-stu-id="f5592-136">int</span></span>      |<span data-ttu-id="f5592-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="f5592-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="f5592-138">$top</span><span class="sxs-lookup"><span data-stu-id="f5592-138">$top</span></span>            |<span data-ttu-id="f5592-139">int</span><span class="sxs-lookup"><span data-stu-id="f5592-139">int</span></span>      |<span data-ttu-id="f5592-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="f5592-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="f5592-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5592-141">Request headers</span></span>

| <span data-ttu-id="f5592-142">Nome</span><span class="sxs-lookup"><span data-stu-id="f5592-142">Name</span></span>           |<span data-ttu-id="f5592-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5592-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f5592-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5592-144">Authorization</span></span>  | <span data-ttu-id="f5592-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5592-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="f5592-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5592-147">Request body</span></span>

<span data-ttu-id="f5592-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5592-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5592-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5592-149">Response</span></span>

<span data-ttu-id="f5592-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5592-150">If successful, this method returns a `200 OK` response code and a collection of [personAnniversary](../resources/personanniversary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5592-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5592-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5592-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5592-152">Request</span></span>

<span data-ttu-id="f5592-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5592-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5592-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5592-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_anniversaries"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/anniversaries
```
# <a name="c"></a>[<span data-ttu-id="f5592-155">C#</span><span class="sxs-lookup"><span data-stu-id="f5592-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-anniversaries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5592-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5592-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-anniversaries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5592-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5592-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-anniversaries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5592-158">Java</span><span class="sxs-lookup"><span data-stu-id="f5592-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-anniversaries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f5592-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5592-159">Response</span></span>
<span data-ttu-id="f5592-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f5592-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personAnniversary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
      "type": "birthday",
      "date": "Date"
    }
  ]
}
```


