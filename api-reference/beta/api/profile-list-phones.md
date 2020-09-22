---
title: Listar telefones
description: Recupere uma lista de objetos de isphone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9f32156a20042ac602576c376e7e1a5ff6eaa48d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034677"
---
# <a name="list-phones"></a><span data-ttu-id="2fba0-103">Listar telefones</span><span class="sxs-lookup"><span data-stu-id="2fba0-103">List phones</span></span>

<span data-ttu-id="2fba0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fba0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fba0-105">Recupere uma lista de objetos de [Multiphone](../resources/itemphone.md) de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="2fba0-105">Retrieve a list of [itemPhone](../resources/itemphone.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2fba0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fba0-106">Permissions</span></span>

<span data-ttu-id="2fba0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fba0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fba0-109">Permission type</span></span>                        | <span data-ttu-id="2fba0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fba0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="2fba0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fba0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fba0-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2fba0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2fba0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fba0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fba0-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2fba0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2fba0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fba0-115">Application</span></span>                            | <span data-ttu-id="2fba0-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2fba0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="2fba0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fba0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones
GET /user/{id | userPrincipalName}/profile/phones
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fba0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2fba0-118">Optional query parameters</span></span>

<span data-ttu-id="2fba0-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2fba0-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="2fba0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2fba0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="2fba0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2fba0-121">Name</span></span>            |<span data-ttu-id="2fba0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2fba0-122">Value</span></span>    |<span data-ttu-id="2fba0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fba0-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="2fba0-124">$filter</span><span class="sxs-lookup"><span data-stu-id="2fba0-124">$filter</span></span>         |<span data-ttu-id="2fba0-125">string</span><span class="sxs-lookup"><span data-stu-id="2fba0-125">string</span></span>   |<span data-ttu-id="2fba0-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="2fba0-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="2fba0-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="2fba0-127">$orderby</span></span>        |<span data-ttu-id="2fba0-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fba0-128">string</span></span>   |<span data-ttu-id="2fba0-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="2fba0-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="2fba0-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="2fba0-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="2fba0-131">$select</span><span class="sxs-lookup"><span data-stu-id="2fba0-131">$select</span></span>         |<span data-ttu-id="2fba0-132">string</span><span class="sxs-lookup"><span data-stu-id="2fba0-132">string</span></span>   |<span data-ttu-id="2fba0-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="2fba0-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="2fba0-135">$skip</span><span class="sxs-lookup"><span data-stu-id="2fba0-135">$skip</span></span>           |<span data-ttu-id="2fba0-136">int</span><span class="sxs-lookup"><span data-stu-id="2fba0-136">int</span></span>      |<span data-ttu-id="2fba0-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="2fba0-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="2fba0-138">$top</span><span class="sxs-lookup"><span data-stu-id="2fba0-138">$top</span></span>            |<span data-ttu-id="2fba0-139">int</span><span class="sxs-lookup"><span data-stu-id="2fba0-139">int</span></span>      |<span data-ttu-id="2fba0-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="2fba0-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="2fba0-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fba0-141">Request headers</span></span>

|<span data-ttu-id="2fba0-142">Nome</span><span class="sxs-lookup"><span data-stu-id="2fba0-142">Name</span></span>|<span data-ttu-id="2fba0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fba0-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2fba0-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fba0-144">Authorization</span></span>|<span data-ttu-id="2fba0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fba0-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fba0-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fba0-147">Request body</span></span>

<span data-ttu-id="2fba0-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fba0-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fba0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fba0-149">Response</span></span>

<span data-ttu-id="2fba0-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [Tel](../resources/itemphone.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fba0-150">If successful, this method returns a `200 OK` response code and a collection of [itemPhone](../resources/itemphone.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2fba0-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2fba0-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2fba0-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fba0-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2fba0-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fba0-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}
-->

``` http
GET https://graph.microsoft.com/beta/me/profile/phones
```
# <a name="c"></a>[<span data-ttu-id="2fba0-154">C#</span><span class="sxs-lookup"><span data-stu-id="2fba0-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fba0-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fba0-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fba0-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fba0-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2fba0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fba0-157">Response</span></span>
<span data-ttu-id="2fba0-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2fba0-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemPhone)"
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
      "displayName": "Car Phone",
      "type": "other",
      "number": "+7 499 342 22 13"
    }
  ]
}
```


