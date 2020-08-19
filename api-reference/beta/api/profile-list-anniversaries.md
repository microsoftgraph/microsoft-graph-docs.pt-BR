---
title: Listar aniversários
description: Recupere uma lista de objetos personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7636ee52a7021845b512bbbdc9ed9100fb7771c8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812834"
---
# <a name="list-anniversaries"></a><span data-ttu-id="12e53-103">Listar aniversários</span><span class="sxs-lookup"><span data-stu-id="12e53-103">List anniversaries</span></span>

<span data-ttu-id="12e53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12e53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12e53-105">Recupere uma lista de objetos [personAnniversary](../resources/personanniversary.md) para o usuário específico do seu [perfil](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="12e53-105">Retrieve a list of [personAnniversary](../resources/personanniversary.md) objects for the given user from their [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="12e53-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12e53-106">Permissions</span></span>

<span data-ttu-id="12e53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12e53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12e53-109">Permission type</span></span>                        | <span data-ttu-id="12e53-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12e53-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="12e53-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12e53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12e53-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="12e53-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="12e53-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12e53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12e53-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="12e53-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="12e53-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12e53-115">Application</span></span>                            | <span data-ttu-id="12e53-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="12e53-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="12e53-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12e53-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/anniversaries
GET /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12e53-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12e53-118">Optional query parameters</span></span>

<span data-ttu-id="12e53-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12e53-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="12e53-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="12e53-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="12e53-121">Nome</span><span class="sxs-lookup"><span data-stu-id="12e53-121">Name</span></span>            |<span data-ttu-id="12e53-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12e53-122">Value</span></span>    |<span data-ttu-id="12e53-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e53-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="12e53-124">$filter</span><span class="sxs-lookup"><span data-stu-id="12e53-124">$filter</span></span>         |<span data-ttu-id="12e53-125">string</span><span class="sxs-lookup"><span data-stu-id="12e53-125">string</span></span>   |<span data-ttu-id="12e53-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="12e53-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="12e53-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="12e53-127">$orderby</span></span>        |<span data-ttu-id="12e53-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12e53-128">string</span></span>   |<span data-ttu-id="12e53-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="12e53-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="12e53-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="12e53-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="12e53-131">$select</span><span class="sxs-lookup"><span data-stu-id="12e53-131">$select</span></span>         |<span data-ttu-id="12e53-132">string</span><span class="sxs-lookup"><span data-stu-id="12e53-132">string</span></span>   |<span data-ttu-id="12e53-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="12e53-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="12e53-135">$skip</span><span class="sxs-lookup"><span data-stu-id="12e53-135">$skip</span></span>           |<span data-ttu-id="12e53-136">int</span><span class="sxs-lookup"><span data-stu-id="12e53-136">int</span></span>      |<span data-ttu-id="12e53-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="12e53-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="12e53-138">$top</span><span class="sxs-lookup"><span data-stu-id="12e53-138">$top</span></span>            |<span data-ttu-id="12e53-139">int</span><span class="sxs-lookup"><span data-stu-id="12e53-139">int</span></span>      |<span data-ttu-id="12e53-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="12e53-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="12e53-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12e53-141">Request headers</span></span>

| <span data-ttu-id="12e53-142">Nome</span><span class="sxs-lookup"><span data-stu-id="12e53-142">Name</span></span>           |<span data-ttu-id="12e53-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e53-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="12e53-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="12e53-144">Authorization</span></span>  | <span data-ttu-id="12e53-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12e53-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="12e53-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12e53-147">Request body</span></span>

<span data-ttu-id="12e53-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12e53-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12e53-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e53-149">Response</span></span>

<span data-ttu-id="12e53-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [personAnniversary](../resources/personanniversary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12e53-150">If successful, this method returns a `200 OK` response code and a collection of [personAnniversary](../resources/personanniversary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12e53-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="12e53-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12e53-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12e53-152">Request</span></span>

<span data-ttu-id="12e53-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12e53-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12e53-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="12e53-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_anniversaries"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/anniversaries
```
# <a name="c"></a>[<span data-ttu-id="12e53-155">C#</span><span class="sxs-lookup"><span data-stu-id="12e53-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-anniversaries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12e53-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12e53-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-anniversaries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12e53-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12e53-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-anniversaries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="12e53-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e53-158">Response</span></span>
<span data-ttu-id="12e53-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="12e53-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
