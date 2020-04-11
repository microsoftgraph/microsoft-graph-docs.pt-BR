---
title: Criar educationalActivity
description: Criar um novo educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da437b7bc53d1d42c2d1f8fcc33d76925c8c8ef
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229343"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="5df24-103">Criar educationalActivity</span><span class="sxs-lookup"><span data-stu-id="5df24-103">Create educationalActivity</span></span>

<span data-ttu-id="5df24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5df24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5df24-105">Criar um novo [educationalActivity](../resources/educationalactivity.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5df24-105">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5df24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5df24-106">Permissions</span></span>

<span data-ttu-id="5df24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5df24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5df24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5df24-109">Permission type</span></span>                        | <span data-ttu-id="5df24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5df24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5df24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5df24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5df24-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5df24-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5df24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5df24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5df24-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5df24-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5df24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5df24-115">Application</span></span>                            | <span data-ttu-id="5df24-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5df24-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5df24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5df24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="5df24-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5df24-118">Request headers</span></span>

| <span data-ttu-id="5df24-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5df24-119">Name</span></span>           |<span data-ttu-id="5df24-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5df24-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5df24-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5df24-121">Authorization</span></span>  | <span data-ttu-id="5df24-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5df24-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5df24-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5df24-124">Content-Type</span></span>   | <span data-ttu-id="5df24-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5df24-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5df24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5df24-127">Request body</span></span>

<span data-ttu-id="5df24-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationalActivity](../resources/educationalactivity.md) .</span><span class="sxs-lookup"><span data-stu-id="5df24-128">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5df24-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5df24-129">Response</span></span>

<span data-ttu-id="5df24-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [educationalActivity](../resources/educationalactivity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5df24-130">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5df24-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5df24-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5df24-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5df24-132">Request</span></span>

<span data-ttu-id="5df24-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5df24-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5df24-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5df24-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5df24-135">C#</span><span class="sxs-lookup"><span data-stu-id="5df24-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationalactivity-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5df24-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5df24-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationalactivity-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5df24-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5df24-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationalactivity-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5df24-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5df24-138">Response</span></span>

<span data-ttu-id="5df24-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5df24-139">The following is an example of the response.</span></span>

> <span data-ttu-id="5df24-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5df24-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
