---
title: Obter personWebsite
description: Recupere as propriedades e os relacionamentos de um objeto personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a72efd0e3f349ecab564f252577b57dd8e69b119
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010658"
---
# <a name="get-personwebsite"></a><span data-ttu-id="905a6-103">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="905a6-103">Get personWebsite</span></span>

<span data-ttu-id="905a6-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="905a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="905a6-105">Recupere as propriedades e os relacionamentos de um objeto [personWebsite](../resources/personwebsite.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="905a6-105">Retrieve the properties and relationships of a [personWebsite](../resources/personwebsite.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="905a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="905a6-106">Permissions</span></span>

<span data-ttu-id="905a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="905a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="905a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="905a6-109">Permission type</span></span>                        | <span data-ttu-id="905a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="905a6-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="905a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="905a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="905a6-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="905a6-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="905a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="905a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="905a6-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="905a6-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="905a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="905a6-115">Application</span></span>                            | <span data-ttu-id="905a6-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="905a6-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="905a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="905a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/websites/{id}
GET /users/{id | userPrincipalName}/profile/websites/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="905a6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="905a6-118">Optional query parameters</span></span>

<span data-ttu-id="905a6-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="905a6-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="905a6-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="905a6-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="905a6-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="905a6-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="905a6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="905a6-122">Request headers</span></span>

| <span data-ttu-id="905a6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="905a6-123">Name</span></span>           |<span data-ttu-id="905a6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="905a6-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="905a6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="905a6-125">Authorization</span></span>  | <span data-ttu-id="905a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="905a6-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="905a6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="905a6-128">Request body</span></span>

<span data-ttu-id="905a6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="905a6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="905a6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="905a6-130">Response</span></span>

<span data-ttu-id="905a6-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [personWebsite](../resources/personwebsite.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="905a6-131">If successful, this method returns a `200 OK` response code and the requested [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="905a6-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="905a6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="905a6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="905a6-133">Request</span></span>

<span data-ttu-id="905a6-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="905a6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="905a6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="905a6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personwebsite"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/websites/{id}
```
# <a name="c"></a>[<span data-ttu-id="905a6-136">C#</span><span class="sxs-lookup"><span data-stu-id="905a6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="905a6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="905a6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="905a6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="905a6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="905a6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="905a6-139">Response</span></span>

<span data-ttu-id="905a6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="905a6-140">The following is an example of the response.</span></span>

> <span data-ttu-id="905a6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="905a6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
    "football"
  ],
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway",
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```


