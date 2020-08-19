---
title: Obter personInterest
description: Recupere as propriedades e os relacionamentos de um objeto personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 96158282c5e5a3c39440b710415bebb3de2eda2e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809176"
---
# <a name="get-personinterest"></a><span data-ttu-id="f1370-103">Obter personInterest</span><span class="sxs-lookup"><span data-stu-id="f1370-103">Get personInterest</span></span>

<span data-ttu-id="f1370-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1370-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1370-105">Recupere as propriedades e os relacionamentos de um objeto [personInterest](../resources/personinterest.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f1370-105">Retrieve the properties and relationships of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1370-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1370-106">Permissions</span></span>

<span data-ttu-id="f1370-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1370-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1370-109">Permission type</span></span>                        | <span data-ttu-id="f1370-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1370-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f1370-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1370-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1370-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1370-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f1370-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1370-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1370-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1370-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f1370-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1370-115">Application</span></span>                            | <span data-ttu-id="f1370-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1370-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f1370-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1370-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests/{id}
GET /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1370-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1370-118">Optional query parameters</span></span>

<span data-ttu-id="f1370-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="f1370-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="f1370-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="f1370-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="f1370-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="f1370-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1370-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1370-122">Request headers</span></span>

| <span data-ttu-id="f1370-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f1370-123">Name</span></span>           |<span data-ttu-id="f1370-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1370-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f1370-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1370-125">Authorization</span></span>  | <span data-ttu-id="f1370-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1370-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="f1370-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1370-128">Request body</span></span>

<span data-ttu-id="f1370-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1370-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1370-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1370-130">Response</span></span>

<span data-ttu-id="f1370-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [personInterest](../resources/personinterest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1370-131">If successful, this method returns a `200 OK` response code and the requested [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1370-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1370-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1370-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1370-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="f1370-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1370-134">HTTP</span></span>](#tab/http)

<span data-ttu-id="f1370-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1370-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_personinterest"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="f1370-136">C#</span><span class="sxs-lookup"><span data-stu-id="f1370-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1370-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1370-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1370-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1370-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f1370-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1370-139">Response</span></span>

<span data-ttu-id="f1370-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1370-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f1370-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1370-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```
