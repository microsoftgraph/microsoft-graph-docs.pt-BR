---
title: Listar usuário transitiva membro
description: Obtenha grupos e funções de diretório dos quais o usuário é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3c2a8f06b02870d2a1f0d021d77883ab7acf1d70
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316245"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="55878-104">Listar usuário transitiva membro</span><span class="sxs-lookup"><span data-stu-id="55878-104">List user transitive memberOf</span></span>

<span data-ttu-id="55878-105">Obtenha grupos e funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="55878-105">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="55878-106">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="55878-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="55878-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="55878-107">Permissions</span></span>

<span data-ttu-id="55878-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55878-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55878-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55878-110">Permission type</span></span>      | <span data-ttu-id="55878-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55878-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55878-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55878-112">Delegated (work or school account)</span></span> | <span data-ttu-id="55878-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55878-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55878-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55878-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55878-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55878-115">Not supported.</span></span>    |
|<span data-ttu-id="55878-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55878-116">Application</span></span> | <span data-ttu-id="55878-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55878-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55878-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55878-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55878-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55878-119">Optional query parameters</span></span>

<span data-ttu-id="55878-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55878-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55878-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55878-121">Request headers</span></span>

| <span data-ttu-id="55878-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55878-122">Header</span></span>       | <span data-ttu-id="55878-123">Valor</span><span class="sxs-lookup"><span data-stu-id="55878-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55878-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="55878-124">Authorization</span></span>  | <span data-ttu-id="55878-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55878-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="55878-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55878-127">Accept</span></span>  | <span data-ttu-id="55878-128">application/json</span><span class="sxs-lookup"><span data-stu-id="55878-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55878-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55878-129">Request body</span></span>

<span data-ttu-id="55878-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55878-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55878-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="55878-131">Response</span></span>

<span data-ttu-id="55878-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55878-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55878-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55878-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="55878-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55878-134">Request</span></span>

<span data-ttu-id="55878-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55878-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="55878-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="55878-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55878-137">C#</span><span class="sxs-lookup"><span data-stu-id="55878-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55878-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55878-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55878-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="55878-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="55878-140">Java</span><span class="sxs-lookup"><span data-stu-id="55878-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55878-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="55878-141">Response</span></span>

<span data-ttu-id="55878-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55878-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
