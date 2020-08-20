---
title: Listar emails
description: Recupere uma lista de objetos de email.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a3ab4f80069131904d9d619e7ddddb72c5a19511
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819446"
---
# <a name="list-emails"></a><span data-ttu-id="9213e-103">Listar emails</span><span class="sxs-lookup"><span data-stu-id="9213e-103">List emails</span></span>

<span data-ttu-id="9213e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9213e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9213e-105">Recupere uma lista de objetos de [email](../resources/itememail.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9213e-105">Retrieve a list of [itemEmail](../resources/itememail.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9213e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9213e-106">Permissions</span></span>

<span data-ttu-id="9213e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9213e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9213e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9213e-109">Permission type</span></span>                        | <span data-ttu-id="9213e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9213e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9213e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9213e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9213e-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9213e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9213e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9213e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9213e-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9213e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9213e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9213e-115">Application</span></span>                            | <span data-ttu-id="9213e-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9213e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9213e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9213e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/emails
GET /users/{id | userPrincipalName}/profile/emails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9213e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9213e-118">Optional query parameters</span></span>

<span data-ttu-id="9213e-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9213e-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="9213e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9213e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="9213e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9213e-121">Name</span></span>            |<span data-ttu-id="9213e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9213e-122">Value</span></span>    |<span data-ttu-id="9213e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9213e-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="9213e-124">$filter</span><span class="sxs-lookup"><span data-stu-id="9213e-124">$filter</span></span>         |<span data-ttu-id="9213e-125">string</span><span class="sxs-lookup"><span data-stu-id="9213e-125">string</span></span>   |<span data-ttu-id="9213e-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="9213e-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="9213e-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="9213e-127">$orderby</span></span>        |<span data-ttu-id="9213e-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9213e-128">string</span></span>   |<span data-ttu-id="9213e-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="9213e-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="9213e-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="9213e-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="9213e-131">$select</span><span class="sxs-lookup"><span data-stu-id="9213e-131">$select</span></span>         |<span data-ttu-id="9213e-132">string</span><span class="sxs-lookup"><span data-stu-id="9213e-132">string</span></span>   |<span data-ttu-id="9213e-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="9213e-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="9213e-135">$skip</span><span class="sxs-lookup"><span data-stu-id="9213e-135">$skip</span></span>           |<span data-ttu-id="9213e-136">int</span><span class="sxs-lookup"><span data-stu-id="9213e-136">int</span></span>      |<span data-ttu-id="9213e-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="9213e-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="9213e-138">$top</span><span class="sxs-lookup"><span data-stu-id="9213e-138">$top</span></span>            |<span data-ttu-id="9213e-139">int</span><span class="sxs-lookup"><span data-stu-id="9213e-139">int</span></span>      |<span data-ttu-id="9213e-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="9213e-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="9213e-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9213e-141">Request headers</span></span>

| <span data-ttu-id="9213e-142">Nome</span><span class="sxs-lookup"><span data-stu-id="9213e-142">Name</span></span>           |<span data-ttu-id="9213e-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="9213e-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="9213e-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="9213e-144">Authorization</span></span>  | <span data-ttu-id="9213e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9213e-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="9213e-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9213e-147">Request body</span></span>
<span data-ttu-id="9213e-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9213e-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9213e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9213e-149">Response</span></span>

<span data-ttu-id="9213e-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [email](../resources/itememail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9213e-150">If successful, this method returns a `200 OK` response code and a collection of [itemEmail](../resources/itememail.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9213e-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9213e-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="9213e-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="9213e-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/emails
```
# <a name="c"></a>[<span data-ttu-id="9213e-153">C#</span><span class="sxs-lookup"><span data-stu-id="9213e-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9213e-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9213e-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9213e-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9213e-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9213e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9213e-156">Response</span></span>

<span data-ttu-id="9213e-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9213e-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Innocenty Popov"
        }
      },
      "lastModifiedDateTime": "2020-07-08T06:34:12.2294868Z",
      "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Innocenty Popov"
        }
      },
      "source": {
        "type": "User"
      },
      "address": "innocenty.popov@adventureworks.com",
      "displayName": "Innocenty Popov",
      "type": "work"
    }
  ]
}
```
