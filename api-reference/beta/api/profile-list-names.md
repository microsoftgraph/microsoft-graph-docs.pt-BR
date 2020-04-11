---
title: Listar nomes
description: Recupere uma lista de objetos PersonName do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 87688a8e8049370ebe6a0bd4929450f3de7a1301
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228657"
---
# <a name="list-names"></a><span data-ttu-id="8985f-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="8985f-103">List names</span></span>

<span data-ttu-id="8985f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8985f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8985f-105">Recupere uma lista de objetos [PersonName](../resources/personname.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8985f-105">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8985f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8985f-106">Permissions</span></span>

<span data-ttu-id="8985f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8985f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8985f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8985f-109">Permission type</span></span>                        | <span data-ttu-id="8985f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8985f-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8985f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8985f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8985f-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8985f-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8985f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8985f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8985f-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8985f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8985f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8985f-115">Application</span></span>                            | <span data-ttu-id="8985f-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8985f-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="8985f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8985f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8985f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8985f-118">Optional query parameters</span></span>

<span data-ttu-id="8985f-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8985f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8985f-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8985f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8985f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8985f-121">Request headers</span></span>

| <span data-ttu-id="8985f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8985f-122">Name</span></span>           |<span data-ttu-id="8985f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8985f-123">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8985f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8985f-124">Authorization</span></span>  | <span data-ttu-id="8985f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8985f-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8985f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8985f-127">Content-Type</span></span>   | <span data-ttu-id="8985f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8985f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8985f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8985f-130">Request body</span></span>

<span data-ttu-id="8985f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8985f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8985f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8985f-132">Response</span></span>

<span data-ttu-id="8985f-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [PersonName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8985f-133">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8985f-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8985f-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8985f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8985f-135">Request</span></span>

<span data-ttu-id="8985f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8985f-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8985f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8985f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names
```
# <a name="c"></a>[<span data-ttu-id="8985f-138">C#</span><span class="sxs-lookup"><span data-stu-id="8985f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8985f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8985f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8985f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8985f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8985f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8985f-141">Response</span></span>

<span data-ttu-id="8985f-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8985f-142">The following is an example of the response.</span></span>

> <span data-ttu-id="8985f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8985f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "first": "first-value",
      "initials": "initials-value",
      "last": "last-value",
      "languageTag": "languageTag-value",
      "maiden": "maiden-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
