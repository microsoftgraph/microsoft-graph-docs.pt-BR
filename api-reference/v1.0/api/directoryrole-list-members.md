---
title: Listar membros
description: Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5bc68b6a0a70a99c24e2f4cedd4ae909f201a13e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459325"
---
# <a name="list-members"></a><span data-ttu-id="e0fbd-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="e0fbd-104">List members</span></span>

<span data-ttu-id="e0fbd-105">Recupera uma lista dos usuários atribuídos à função de diretório.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="e0fbd-106">Somente usuários podem ser atribuídos a uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0fbd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0fbd-107">Permissions</span></span>
<span data-ttu-id="e0fbd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0fbd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0fbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0fbd-110">Permission type</span></span>      | <span data-ttu-id="e0fbd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0fbd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0fbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0fbd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0fbd-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0fbd-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0fbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0fbd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0fbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-115">Not supported.</span></span>    |
|<span data-ttu-id="e0fbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0fbd-116">Application</span></span> | <span data-ttu-id="e0fbd-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0fbd-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0fbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0fbd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0fbd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0fbd-119">Optional query parameters</span></span>
<span data-ttu-id="e0fbd-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e0fbd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fbd-121">Request headers</span></span>
| <span data-ttu-id="e0fbd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e0fbd-122">Name</span></span>       | <span data-ttu-id="e0fbd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0fbd-123">Type</span></span> | <span data-ttu-id="e0fbd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0fbd-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0fbd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0fbd-125">Authorization</span></span>  | <span data-ttu-id="e0fbd-126">string</span><span class="sxs-lookup"><span data-stu-id="e0fbd-126">string</span></span>  | <span data-ttu-id="e0fbd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0fbd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fbd-129">Request body</span></span>
<span data-ttu-id="e0fbd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0fbd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0fbd-131">Response</span></span>

<span data-ttu-id="e0fbd-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0fbd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0fbd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0fbd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0fbd-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e0fbd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0fbd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0fbd-136">C#</span><span class="sxs-lookup"><span data-stu-id="e0fbd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0fbd-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0fbd-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0fbd-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e0fbd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0fbd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0fbd-139">Response</span></span>
<span data-ttu-id="e0fbd-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0fbd-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
