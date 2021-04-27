---
title: Obter personName
description: Recupere as propriedades e as relações de um objeto personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 06e61b98f4af32f5c1f599effe3fa7124003738a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050056"
---
# <a name="get-personname"></a><span data-ttu-id="d449d-103">Obter personName</span><span class="sxs-lookup"><span data-stu-id="d449d-103">Get personName</span></span>

<span data-ttu-id="d449d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d449d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d449d-105">Recupere as propriedades e as relações de um [objeto personName](../resources/personname.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="d449d-105">Retrieve the properties and relationships of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d449d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d449d-106">Permissions</span></span>

<span data-ttu-id="d449d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d449d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d449d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d449d-109">Permission type</span></span>                        | <span data-ttu-id="d449d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d449d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d449d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d449d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d449d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d449d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d449d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d449d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d449d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d449d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d449d-115">Application</span><span class="sxs-lookup"><span data-stu-id="d449d-115">Application</span></span>                            | <span data-ttu-id="d449d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d449d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d449d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d449d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names/{id}
GET /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d449d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d449d-118">Optional query parameters</span></span>

<span data-ttu-id="d449d-119">Este método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="d449d-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="d449d-120">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="d449d-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="d449d-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="d449d-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d449d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d449d-122">Request headers</span></span>

| <span data-ttu-id="d449d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d449d-123">Name</span></span>           |<span data-ttu-id="d449d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d449d-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d449d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d449d-125">Authorization</span></span>  | <span data-ttu-id="d449d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d449d-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d449d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d449d-128">Content-Type</span></span>   | <span data-ttu-id="d449d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d449d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d449d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d449d-131">Request body</span></span>

<span data-ttu-id="d449d-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d449d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d449d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d449d-133">Response</span></span>

<span data-ttu-id="d449d-134">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [personName](../resources/personname.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d449d-134">If successful, this method returns a `200 OK` response code and the requested [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d449d-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d449d-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d449d-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d449d-136">Request</span></span>

<span data-ttu-id="d449d-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d449d-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d449d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d449d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personname"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="c"></a>[<span data-ttu-id="d449d-139">C#</span><span class="sxs-lookup"><span data-stu-id="d449d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d449d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d449d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d449d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d449d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d449d-142">Java</span><span class="sxs-lookup"><span data-stu-id="d449d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d449d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d449d-143">Response</span></span>

<span data-ttu-id="d449d-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d449d-144">The following is an example of the response.</span></span>

> <span data-ttu-id="d449d-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d449d-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
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
```


