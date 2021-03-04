---
title: Obter userAccountInformation
description: Recupere as propriedades e as relações do objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: ec6b24daf3b2314e8175a7456f3187f2ac67178c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443297"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="e3f3e-103">Obter userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="e3f3e-103">Get userAccountInformation</span></span>

<span data-ttu-id="e3f3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f3e-105">Recupere as propriedades e as relações de [um objeto userAccountInformation](../resources/useraccountinformation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e3f3e-105">Retrieve the properties and relationships of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3f3e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3f3e-106">Permissions</span></span>

<span data-ttu-id="e3f3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3f3e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3f3e-109">Permission type</span></span>                        | <span data-ttu-id="e3f3e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3f3e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e3f3e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3f3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3f3e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f3e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e3f3e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3f3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3f3e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f3e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e3f3e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3f3e-115">Application</span></span>                            | <span data-ttu-id="e3f3e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f3e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e3f3e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3f3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account/{id}
GET /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3f3e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3f3e-118">Optional query parameters</span></span>

<span data-ttu-id="e3f3e-119">Este método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="e3f3e-120">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="e3f3e-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3f3e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f3e-122">Request headers</span></span>

| <span data-ttu-id="e3f3e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e3f3e-123">Name</span></span>          |<span data-ttu-id="e3f3e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3f3e-124">Description</span></span>                |
|:--------------|:--------------------------|
| <span data-ttu-id="e3f3e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3f3e-125">Authorization</span></span> | <span data-ttu-id="e3f3e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3f3e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f3e-128">Request body</span></span>

<span data-ttu-id="e3f3e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3f3e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3f3e-130">Response</span></span>

<span data-ttu-id="e3f3e-131">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [userAccountInformation](../resources/useraccountinformation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-131">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3f3e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3f3e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3f3e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f3e-133">Request</span></span>

<span data-ttu-id="e3f3e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3f3e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3f3e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account/{id}
```
# <a name="c"></a>[<span data-ttu-id="e3f3e-136">C#</span><span class="sxs-lookup"><span data-stu-id="e3f3e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3f3e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3f3e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3f3e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3f3e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3f3e-139">Java</span><span class="sxs-lookup"><span data-stu-id="e3f3e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3f3e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3f3e-140">Response</span></span>

<span data-ttu-id="e3f3e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="e3f3e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3f3e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
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
  "source": null,
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


