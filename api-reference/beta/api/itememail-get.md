---
title: Obter email
description: Recupere as propriedades e os relacionamentos de um objeto de item de email.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4e009cc138e4a6560ad5b7c69ad6a5c9425d17ee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969992"
---
# <a name="get-itememail"></a><span data-ttu-id="cfa0e-103">Obter email</span><span class="sxs-lookup"><span data-stu-id="cfa0e-103">Get itemEmail</span></span>

<span data-ttu-id="cfa0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfa0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfa0e-105">Recupere as propriedades e os relacionamentos de um objeto de item de [email](../resources/itememail.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-105">Retrieve the properties and relationships of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfa0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfa0e-106">Permissions</span></span>

<span data-ttu-id="cfa0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfa0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfa0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfa0e-109">Permission type</span></span>                        | <span data-ttu-id="cfa0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfa0e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="cfa0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfa0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfa0e-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cfa0e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cfa0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfa0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfa0e-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cfa0e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cfa0e-115">Application</span><span class="sxs-lookup"><span data-stu-id="cfa0e-115">Application</span></span>                            | <span data-ttu-id="cfa0e-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cfa0e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="cfa0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfa0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/emails/{id}
GET /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfa0e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cfa0e-118">Optional query parameters</span></span>

<span data-ttu-id="cfa0e-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="cfa0e-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="cfa0e-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfa0e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfa0e-122">Request headers</span></span>
|<span data-ttu-id="cfa0e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cfa0e-123">Name</span></span>|<span data-ttu-id="cfa0e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfa0e-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cfa0e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfa0e-125">Authorization</span></span>|<span data-ttu-id="cfa0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfa0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfa0e-128">Request body</span></span>
<span data-ttu-id="cfa0e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfa0e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfa0e-130">Response</span></span>

<span data-ttu-id="cfa0e-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [email](../resources/itememail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-131">If successful, this method returns a `200 OK` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfa0e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cfa0e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfa0e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfa0e-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="cfa0e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfa0e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itememail"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/profile/emails/{id}
```
# <a name="c"></a>[<span data-ttu-id="cfa0e-135">C#</span><span class="sxs-lookup"><span data-stu-id="cfa0e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfa0e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfa0e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfa0e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfa0e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfa0e-138">Java</span><span class="sxs-lookup"><span data-stu-id="cfa0e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itememail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cfa0e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfa0e-139">Response</span></span>
<span data-ttu-id="cfa0e-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cfa0e-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": "Business Email",
  "type": "work"
}
```


