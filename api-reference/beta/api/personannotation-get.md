---
title: Obter personAnnotation
description: Leia as propriedades e os relacionamentos de um objeto personAnnotation.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2d13769f6b9493d049496bbebd895e6516427266
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968385"
---
# <a name="get-personannotation"></a><span data-ttu-id="b7f9d-103">Obter personAnnotation</span><span class="sxs-lookup"><span data-stu-id="b7f9d-103">Get personAnnotation</span></span>
<span data-ttu-id="b7f9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7f9d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7f9d-105">Leia as propriedades e os relacionamentos de um objeto [personAnnotation](../resources/personannotation.md) a partir de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-105">Read the properties and relationships of a [personAnnotation](../resources/personannotation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f9d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7f9d-106">Permissions</span></span>

<span data-ttu-id="b7f9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7f9d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7f9d-109">Permission type</span></span>                        | <span data-ttu-id="b7f9d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7f9d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b7f9d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7f9d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7f9d-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7f9d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b7f9d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7f9d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f9d-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7f9d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b7f9d-115">Application</span><span class="sxs-lookup"><span data-stu-id="b7f9d-115">Application</span></span>                            | <span data-ttu-id="b7f9d-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7f9d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b7f9d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7f9d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/notes/{id}
GET /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7f9d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7f9d-118">Optional query parameters</span></span>

<span data-ttu-id="b7f9d-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="b7f9d-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="b7f9d-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7f9d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f9d-122">Request headers</span></span>
|<span data-ttu-id="b7f9d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b7f9d-123">Name</span></span>|<span data-ttu-id="b7f9d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f9d-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7f9d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7f9d-125">Authorization</span></span>|<span data-ttu-id="b7f9d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f9d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f9d-128">Request body</span></span>
<span data-ttu-id="b7f9d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7f9d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f9d-130">Response</span></span>

<span data-ttu-id="b7f9d-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [personAnnotation](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-131">If successful, this method returns a `200 OK` response code and a [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7f9d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7f9d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7f9d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f9d-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="b7f9d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7f9d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personannotation"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/notes/{id}
```
# <a name="c"></a>[<span data-ttu-id="b7f9d-135">C#</span><span class="sxs-lookup"><span data-stu-id="b7f9d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personannotation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7f9d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7f9d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personannotation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7f9d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7f9d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personannotation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7f9d-138">Java</span><span class="sxs-lookup"><span data-stu-id="b7f9d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-personannotation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b7f9d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f9d-139">Response</span></span>
<span data-ttu-id="b7f9d-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b7f9d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnnotation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow."
  },
  "displayName": "About Me"
}
```


