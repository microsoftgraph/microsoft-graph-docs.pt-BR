---
title: Listar usuário transitiva membro
description: Obtenha grupos e funções de diretório dos quais o usuário é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ac0819c970fa1e2c5e17fda29fd68bb35105f01b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274001"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="6c4da-104">Listar usuário transitiva membro</span><span class="sxs-lookup"><span data-stu-id="6c4da-104">List user transitive memberOf</span></span>

<span data-ttu-id="6c4da-105">Obtenha grupos e funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="6c4da-105">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="6c4da-106">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="6c4da-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c4da-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c4da-107">Permissions</span></span>

<span data-ttu-id="6c4da-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c4da-110">Permission type</span></span>      | <span data-ttu-id="6c4da-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c4da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c4da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c4da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c4da-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c4da-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c4da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c4da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c4da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c4da-115">Not supported.</span></span>    |
|<span data-ttu-id="6c4da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c4da-116">Application</span></span> | <span data-ttu-id="6c4da-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c4da-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c4da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c4da-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c4da-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c4da-119">Optional query parameters</span></span>

<span data-ttu-id="6c4da-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c4da-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c4da-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c4da-121">Request headers</span></span>

| <span data-ttu-id="6c4da-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c4da-122">Header</span></span>       | <span data-ttu-id="6c4da-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6c4da-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c4da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c4da-124">Authorization</span></span>  | <span data-ttu-id="6c4da-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c4da-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c4da-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c4da-127">Accept</span></span>  | <span data-ttu-id="6c4da-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6c4da-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c4da-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c4da-129">Request body</span></span>

<span data-ttu-id="6c4da-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c4da-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c4da-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c4da-131">Response</span></span>

<span data-ttu-id="6c4da-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c4da-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c4da-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c4da-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c4da-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c4da-134">Request</span></span>

<span data-ttu-id="6c4da-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c4da-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="6c4da-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c4da-136">Response</span></span>

<span data-ttu-id="6c4da-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c4da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c4da-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6c4da-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c4da-141">C#</span><span class="sxs-lookup"><span data-stu-id="6c4da-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c4da-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c4da-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6c4da-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6c4da-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
