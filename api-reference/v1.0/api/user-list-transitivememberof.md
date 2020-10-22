---
title: Listar usuário transitivo memberOf
description: Obtenha grupos e funções de diretório dos quais o usuário é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 935e5e507c2f6f9a231a5b6a57160899fe60dc56
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634946"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="2e47e-104">Listar usuário transitivo memberOf</span><span class="sxs-lookup"><span data-stu-id="2e47e-104">List user transitive memberOf</span></span>

<span data-ttu-id="2e47e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e47e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e47e-106">Obtenha grupos e funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="2e47e-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="2e47e-107">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="2e47e-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e47e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e47e-108">Permissions</span></span>

<span data-ttu-id="2e47e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e47e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e47e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e47e-111">Permission type</span></span>      | <span data-ttu-id="2e47e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e47e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e47e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e47e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2e47e-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e47e-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e47e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e47e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e47e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e47e-116">Not supported.</span></span>    |
|<span data-ttu-id="2e47e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e47e-117">Application</span></span> | <span data-ttu-id="2e47e-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e47e-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2e47e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e47e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e47e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e47e-120">Optional query parameters</span></span>

<span data-ttu-id="2e47e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e47e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e47e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e47e-122">Request headers</span></span>

| <span data-ttu-id="2e47e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e47e-123">Header</span></span>       | <span data-ttu-id="2e47e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2e47e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e47e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e47e-125">Authorization</span></span>  | <span data-ttu-id="2e47e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e47e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e47e-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e47e-128">Accept</span></span>  | <span data-ttu-id="2e47e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2e47e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e47e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e47e-130">Request body</span></span>

<span data-ttu-id="2e47e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e47e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e47e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e47e-132">Response</span></span>

<span data-ttu-id="2e47e-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e47e-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e47e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e47e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e47e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e47e-135">Request</span></span>

<span data-ttu-id="2e47e-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e47e-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e47e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e47e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="2e47e-138">C#</span><span class="sxs-lookup"><span data-stu-id="2e47e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e47e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e47e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e47e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e47e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e47e-141">Java</span><span class="sxs-lookup"><span data-stu-id="2e47e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e47e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e47e-142">Response</span></span>

<span data-ttu-id="2e47e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e47e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
