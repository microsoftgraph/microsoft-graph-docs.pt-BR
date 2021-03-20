---
title: Obter perfil
description: Recupere as propriedades e as relações do objeto profile.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5e75302cb787a898a0dd7b02498e99b898222fcb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950597"
---
# <a name="get-profile"></a><span data-ttu-id="f6107-103">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="f6107-103">Get profile</span></span>

<span data-ttu-id="f6107-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6107-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6107-105">Recupere as propriedades e as relações de um [objeto de perfil](../resources/profile.md) para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="f6107-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="f6107-106">O **recurso** de perfil expõe várias propriedades ricas que são [descritivas](../resources/profile.md#relationships)do usuário como relações , por exemplo, aniversários e atividades de educação.</span><span class="sxs-lookup"><span data-stu-id="f6107-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="f6107-107">Para obter uma dessas propriedades de navegação, use o método GET correspondente nessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="f6107-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="f6107-108">Consulte os [métodos expostos](../resources/profile.md) pelo **perfil**.</span><span class="sxs-lookup"><span data-stu-id="f6107-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6107-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6107-109">Permissions</span></span>

<span data-ttu-id="f6107-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6107-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6107-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6107-112">Permission type</span></span>                        | <span data-ttu-id="f6107-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6107-113">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f6107-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6107-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6107-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6107-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f6107-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6107-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6107-117">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6107-117">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f6107-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6107-118">Application</span></span>                            | <span data-ttu-id="f6107-119">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6107-119">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f6107-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6107-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
GET /users/{id | userPrincipalName}/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6107-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6107-121">Optional query parameters</span></span>

<span data-ttu-id="f6107-122">Este método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="f6107-122">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="f6107-123">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="f6107-123">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="f6107-124">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="f6107-124">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6107-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6107-125">Request headers</span></span>

| <span data-ttu-id="f6107-126">Nome</span><span class="sxs-lookup"><span data-stu-id="f6107-126">Name</span></span>           |<span data-ttu-id="f6107-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6107-127">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f6107-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6107-128">Authorization</span></span>  | <span data-ttu-id="f6107-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6107-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f6107-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6107-131">Content-Type</span></span>   | <span data-ttu-id="f6107-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6107-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6107-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6107-134">Request body</span></span>

<span data-ttu-id="f6107-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6107-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6107-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6107-136">Response</span></span>

<span data-ttu-id="f6107-137">Se tiver êxito, este método retornará um código de resposta e o objeto de perfil `200 OK` solicitado no corpo da resposta. [](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="f6107-137">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6107-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f6107-138">Examples</span></span>

### <a name="example-1-get-a-users-profile"></a><span data-ttu-id="f6107-139">Exemplo 1: OBTER o perfil de um usuário</span><span class="sxs-lookup"><span data-stu-id="f6107-139">Example 1: GET a user's profile</span></span>

<span data-ttu-id="f6107-140">A seguir, um exemplo da solicitação de perfil GET.</span><span class="sxs-lookup"><span data-stu-id="f6107-140">The following is an example of the GET profile request.</span></span>

#### <a name="request"></a><span data-ttu-id="f6107-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6107-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6107-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6107-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="f6107-143">C#</span><span class="sxs-lookup"><span data-stu-id="f6107-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6107-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6107-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6107-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6107-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6107-146">Java</span><span class="sxs-lookup"><span data-stu-id="f6107-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profile-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f6107-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6107-147">Response</span></span>

<span data-ttu-id="f6107-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6107-148">The following is an example of the response.</span></span>

> <span data-ttu-id="f6107-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6107-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "34545-32444234-2334452-234332-432234",
  "accounts": [],
  "addresses": [
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
      "displayName": "Home",
      "detail": {
        "type": "home",
        "postOfficeBox": null,
        "street": "221B Baker Street",
        "city": "London",
        "state": null,
        "countryOrRegion": "United Kingdom",
        "postalCode": "E14 3TD"
      },
      "geoCoordinates": null
    }
  ],
  "anniversaries": [
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
  ],
  "websites": [],
  "educationalActivities": [],
  "emails": [
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
  ],
  "notes": [],
  "interests": [],
  "languages": [],
  "names": [
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
  ],
  "phones": [
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
  ],
  "positions": [],
  "projects": [],
  "skills": [],
  "webAccounts": []
}
```

### <a name="example-2-expand-names-and-skills-collection-and-select-properties-within-the-entities"></a><span data-ttu-id="f6107-151">Exemplo 2: Expanda nomes e conjunto de habilidades e selecione propriedades dentro das entidades</span><span class="sxs-lookup"><span data-stu-id="f6107-151">Example 2: Expand names and skills collection and select properties within the entities</span></span>

<span data-ttu-id="f6107-152">A seguir, um exemplo de uso dos parâmetros de $expand e $select de consulta para recuperar informações parciais do perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f6107-152">The following is an example of using the $expand and $select query parameters to retrieve partial information from a user's profile.</span></span>

#### <a name="request"></a><span data-ttu-id="f6107-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6107-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6107-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6107-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile?$expand=names($select=first,last),skills($select=displayName)
```
# <a name="c"></a>[<span data-ttu-id="f6107-155">C#</span><span class="sxs-lookup"><span data-stu-id="f6107-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6107-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6107-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6107-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6107-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6107-158">Java</span><span class="sxs-lookup"><span data-stu-id="f6107-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profile-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f6107-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6107-159">Response</span></span>

<span data-ttu-id="f6107-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6107-160">The following is an example of the response.</span></span>

> <span data-ttu-id="f6107-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6107-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "34545-32444234-2334452-234332-432234",
  "names": [
      {
          "first": "Innocenty",
          "last": "Popov"
      }
  ],
  "skills": [
      {
          "displayName": "Machine Learning"
      },
      {
          "displayName": "Artificial Intelligence"
      }
  ]
}
```


