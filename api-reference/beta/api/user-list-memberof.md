---
title: Listar usuário membro
description: Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto. Essa operação não é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 20f09dd162cb36695cc629987722543707a62e22
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637231"
---
# <a name="list-user-memberof"></a><span data-ttu-id="6fb1a-104">Listar usuário membro</span><span class="sxs-lookup"><span data-stu-id="6fb1a-104">List user memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb1a-105">Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-105">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="6fb1a-106">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fb1a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fb1a-107">Permissions</span></span>

<span data-ttu-id="6fb1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fb1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fb1a-110">Permission type</span></span>      | <span data-ttu-id="6fb1a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fb1a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fb1a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb1a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6fb1a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6fb1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fb1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-115">Not supported.</span></span>    |
|<span data-ttu-id="6fb1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fb1a-116">Application</span></span> | <span data-ttu-id="6fb1a-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb1a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fb1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb1a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fb1a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6fb1a-119">Optional query parameters</span></span>

<span data-ttu-id="6fb1a-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6fb1a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb1a-121">Request headers</span></span>
| <span data-ttu-id="6fb1a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fb1a-122">Header</span></span>       | <span data-ttu-id="6fb1a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6fb1a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fb1a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fb1a-124">Authorization</span></span>  | <span data-ttu-id="6fb1a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6fb1a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6fb1a-127">Accept</span></span>  | <span data-ttu-id="6fb1a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6fb1a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb1a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb1a-129">Request body</span></span>

<span data-ttu-id="6fb1a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb1a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb1a-131">Response</span></span>

<span data-ttu-id="6fb1a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fb1a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fb1a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fb1a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb1a-134">Request</span></span>

<span data-ttu-id="6fb1a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/me/memberOf
```

### <a name="response"></a><span data-ttu-id="6fb1a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb1a-136">Response</span></span>

<span data-ttu-id="6fb1a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fb1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6fb1a-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6fb1a-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6fb1a-141">Basic</span><span class="sxs-lookup"><span data-stu-id="6fb1a-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_user_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fb1a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fb1a-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_user_memberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
