---
title: Obter o número de telefone
description: Recupere as propriedades e os relacionamentos de um objeto MyPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: de5c8b733cc26ee6ac4a08a45326eaab8687804b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998294"
---
# <a name="get-itemphonenumber"></a><span data-ttu-id="da263-103">Obter itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="da263-103">Get itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da263-104">Recupere as propriedades e os relacionamentos de um objeto [MyPhone](../resources/itemphone.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="da263-104">Retrieve the properties and relationships of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="da263-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da263-105">Permissions</span></span>

<span data-ttu-id="da263-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da263-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da263-108">Permission type</span></span>                        | <span data-ttu-id="da263-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da263-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="da263-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da263-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="da263-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="da263-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="da263-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da263-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da263-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="da263-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="da263-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da263-114">Application</span></span>                            | <span data-ttu-id="da263-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="da263-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="da263-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da263-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones/{id} 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da263-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da263-117">Optional query parameters</span></span>

<span data-ttu-id="da263-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da263-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="da263-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da263-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="da263-120">Nome</span><span class="sxs-lookup"><span data-stu-id="da263-120">Name</span></span>            |<span data-ttu-id="da263-121">Valor</span><span class="sxs-lookup"><span data-stu-id="da263-121">Value</span></span>    |<span data-ttu-id="da263-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="da263-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="da263-123">$filter</span><span class="sxs-lookup"><span data-stu-id="da263-123">$filter</span></span>         |<span data-ttu-id="da263-124">string</span><span class="sxs-lookup"><span data-stu-id="da263-124">string</span></span>   |<span data-ttu-id="da263-125">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="da263-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="da263-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="da263-126">$orderby</span></span>        |<span data-ttu-id="da263-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da263-127">string</span></span>   |<span data-ttu-id="da263-128">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="da263-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="da263-129">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="da263-129">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="da263-130">$select</span><span class="sxs-lookup"><span data-stu-id="da263-130">$select</span></span>         |<span data-ttu-id="da263-131">string</span><span class="sxs-lookup"><span data-stu-id="da263-131">string</span></span>   |<span data-ttu-id="da263-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="da263-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="da263-134">$skip</span><span class="sxs-lookup"><span data-stu-id="da263-134">$skip</span></span>           |<span data-ttu-id="da263-135">int</span><span class="sxs-lookup"><span data-stu-id="da263-135">int</span></span>      |<span data-ttu-id="da263-136">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="da263-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="da263-137">$top</span><span class="sxs-lookup"><span data-stu-id="da263-137">$top</span></span>            |<span data-ttu-id="da263-138">int</span><span class="sxs-lookup"><span data-stu-id="da263-138">int</span></span>      |<span data-ttu-id="da263-139">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="da263-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="da263-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da263-140">Request headers</span></span>

| <span data-ttu-id="da263-141">Nome</span><span class="sxs-lookup"><span data-stu-id="da263-141">Name</span></span>           |<span data-ttu-id="da263-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="da263-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="da263-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="da263-143">Authorization</span></span>  | <span data-ttu-id="da263-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da263-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="da263-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da263-146">Request body</span></span>

<span data-ttu-id="da263-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da263-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da263-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="da263-148">Response</span></span>

<span data-ttu-id="da263-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [MyPhone](../resources/itemphone.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da263-149">If successful, this method returns a `200 OK` response code and the requested [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da263-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da263-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da263-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da263-151">Request</span></span>

<span data-ttu-id="da263-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da263-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da263-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="da263-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/phones/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da263-154">C#</span><span class="sxs-lookup"><span data-stu-id="da263-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da263-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da263-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da263-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da263-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da263-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="da263-157">Response</span></span>

<span data-ttu-id="da263-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da263-158">The following is an example of the response.</span></span>

> <span data-ttu-id="da263-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da263-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
