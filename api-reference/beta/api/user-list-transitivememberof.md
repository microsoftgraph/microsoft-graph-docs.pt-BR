---
title: Listar usuário transitiva membro
description: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c33210e42d3334feec8c1c06be162e673e3c3b94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451753"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="486aa-104">Listar usuário transitiva membro</span><span class="sxs-lookup"><span data-stu-id="486aa-104">List user transitive memberOf</span></span>

<span data-ttu-id="486aa-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="486aa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="486aa-106">Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="486aa-106">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="486aa-107">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="486aa-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="486aa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="486aa-108">Permissions</span></span>

<span data-ttu-id="486aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="486aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="486aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="486aa-111">Permission type</span></span>      | <span data-ttu-id="486aa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="486aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="486aa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="486aa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="486aa-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="486aa-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="486aa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="486aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="486aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="486aa-116">Not supported.</span></span>    |
|<span data-ttu-id="486aa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="486aa-117">Application</span></span> | <span data-ttu-id="486aa-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="486aa-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="486aa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="486aa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="486aa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="486aa-120">Optional query parameters</span></span>

<span data-ttu-id="486aa-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="486aa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="486aa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="486aa-122">Request headers</span></span>

| <span data-ttu-id="486aa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="486aa-123">Header</span></span>       | <span data-ttu-id="486aa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="486aa-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="486aa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="486aa-125">Authorization</span></span>  | <span data-ttu-id="486aa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="486aa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="486aa-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="486aa-128">Accept</span></span>  | <span data-ttu-id="486aa-129">application/json</span><span class="sxs-lookup"><span data-stu-id="486aa-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="486aa-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="486aa-130">Request body</span></span>

<span data-ttu-id="486aa-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="486aa-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="486aa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="486aa-132">Response</span></span>

<span data-ttu-id="486aa-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="486aa-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="486aa-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="486aa-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="486aa-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="486aa-135">Request</span></span>

<span data-ttu-id="486aa-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="486aa-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="486aa-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="486aa-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="486aa-138">C#</span><span class="sxs-lookup"><span data-stu-id="486aa-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="486aa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="486aa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="486aa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="486aa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="486aa-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="486aa-141">Response</span></span>

<span data-ttu-id="486aa-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="486aa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
