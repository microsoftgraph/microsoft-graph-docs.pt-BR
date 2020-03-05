---
title: Listar aniversários
description: Recupere uma lista de objetos personanniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2da148080d519e6be25b1d8c8bc787061e73f579
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455211"
---
# <a name="list-anniversaries"></a><span data-ttu-id="ecb8a-103">Listar aniversários</span><span class="sxs-lookup"><span data-stu-id="ecb8a-103">List anniversaries</span></span>

<span data-ttu-id="ecb8a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ecb8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecb8a-105">Recupera uma lista de objetos [personAnniversary](../resources/personanniversary.md) para o usuário específico do seu [perfil](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="ecb8a-105">Retrieves a list of the [personAnniversary](../resources/personanniversary.md) objects for the given user from their [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ecb8a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecb8a-106">Permissions</span></span>

<span data-ttu-id="ecb8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecb8a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecb8a-109">Permission type</span></span>                        | <span data-ttu-id="ecb8a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecb8a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ecb8a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecb8a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecb8a-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ecb8a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ecb8a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecb8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb8a-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ecb8a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ecb8a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecb8a-115">Application</span></span>                            | <span data-ttu-id="ecb8a-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ecb8a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ecb8a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecb8a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/anniversaries 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecb8a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecb8a-118">Optional query parameters</span></span>

<span data-ttu-id="ecb8a-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="ecb8a-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ecb8a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="ecb8a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ecb8a-121">Name</span></span>            |<span data-ttu-id="ecb8a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ecb8a-122">Value</span></span>    |<span data-ttu-id="ecb8a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecb8a-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ecb8a-124">$filter</span><span class="sxs-lookup"><span data-stu-id="ecb8a-124">$filter</span></span>         |<span data-ttu-id="ecb8a-125">string</span><span class="sxs-lookup"><span data-stu-id="ecb8a-125">string</span></span>   |<span data-ttu-id="ecb8a-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="ecb8a-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="ecb8a-127">$orderby</span></span>        |<span data-ttu-id="ecb8a-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecb8a-128">string</span></span>   |<span data-ttu-id="ecb8a-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="ecb8a-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="ecb8a-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="ecb8a-131">$select</span><span class="sxs-lookup"><span data-stu-id="ecb8a-131">$select</span></span>         |<span data-ttu-id="ecb8a-132">string</span><span class="sxs-lookup"><span data-stu-id="ecb8a-132">string</span></span>   |<span data-ttu-id="ecb8a-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="ecb8a-135">$skip</span><span class="sxs-lookup"><span data-stu-id="ecb8a-135">$skip</span></span>           |<span data-ttu-id="ecb8a-136">int</span><span class="sxs-lookup"><span data-stu-id="ecb8a-136">int</span></span>      |<span data-ttu-id="ecb8a-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="ecb8a-138">$top</span><span class="sxs-lookup"><span data-stu-id="ecb8a-138">$top</span></span>            |<span data-ttu-id="ecb8a-139">int</span><span class="sxs-lookup"><span data-stu-id="ecb8a-139">int</span></span>      |<span data-ttu-id="ecb8a-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="ecb8a-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecb8a-141">Request headers</span></span>

| <span data-ttu-id="ecb8a-142">Nome</span><span class="sxs-lookup"><span data-stu-id="ecb8a-142">Name</span></span>           |<span data-ttu-id="ecb8a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecb8a-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ecb8a-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecb8a-144">Authorization</span></span>  | <span data-ttu-id="ecb8a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="ecb8a-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecb8a-147">Request body</span></span>

<span data-ttu-id="ecb8a-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb8a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecb8a-149">Response</span></span>

<span data-ttu-id="ecb8a-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-150">If successful, this method returns a `200 OK` response code and a collection of [personAnniversary](../resources/personanniversary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecb8a-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ecb8a-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecb8a-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecb8a-152">Request</span></span>

<span data-ttu-id="ecb8a-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ecb8a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecb8a-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_anniversaries"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/anniversaries
```
# <a name="c"></a>[<span data-ttu-id="ecb8a-155">C#</span><span class="sxs-lookup"><span data-stu-id="ecb8a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-anniversaries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecb8a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecb8a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-anniversaries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecb8a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecb8a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-anniversaries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecb8a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecb8a-158">Response</span></span>

<span data-ttu-id="ecb8a-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-159">The following is an example of the response.</span></span>

> <span data-ttu-id="ecb8a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecb8a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "type": "type-value",
      "date": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List anniversaries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
