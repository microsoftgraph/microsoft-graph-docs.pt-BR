---
title: Lista de grupos transitivos transitivos
description: Obter grupos dos quais o grupo é membro.  Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado. Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a02dd7e4ae4c65132decc6f9f2887bfd91c6d9e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517030"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="ecbef-105">Lista de grupos transitivos transitivos</span><span class="sxs-lookup"><span data-stu-id="ecbef-105">List group transitive memberOf</span></span>

<span data-ttu-id="ecbef-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecbef-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecbef-107">Obter grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="ecbef-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="ecbef-108">Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="ecbef-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="ecbef-109">Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ecbef-109">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecbef-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecbef-110">Permissions</span></span>

<span data-ttu-id="ecbef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecbef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecbef-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecbef-113">Permission type</span></span>      | <span data-ttu-id="ecbef-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecbef-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecbef-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecbef-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ecbef-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ecbef-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ecbef-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecbef-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecbef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecbef-118">Not supported.</span></span>    |
|<span data-ttu-id="ecbef-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecbef-119">Application</span></span> | <span data-ttu-id="ecbef-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecbef-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ecbef-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecbef-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecbef-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ecbef-122">Optional query parameters</span></span>
<span data-ttu-id="ecbef-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ecbef-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecbef-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecbef-124">Request headers</span></span>
| <span data-ttu-id="ecbef-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ecbef-125">Name</span></span>       | <span data-ttu-id="ecbef-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecbef-126">Type</span></span> | <span data-ttu-id="ecbef-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecbef-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ecbef-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecbef-128">Authorization</span></span>  | <span data-ttu-id="ecbef-129">string</span><span class="sxs-lookup"><span data-stu-id="ecbef-129">string</span></span>  | <span data-ttu-id="ecbef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecbef-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecbef-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecbef-132">Request body</span></span>
<span data-ttu-id="ecbef-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecbef-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecbef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecbef-134">Response</span></span>
<span data-ttu-id="ecbef-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecbef-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecbef-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecbef-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecbef-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecbef-137">Request</span></span>
<span data-ttu-id="ecbef-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecbef-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ecbef-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecbef-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="ecbef-140">C#</span><span class="sxs-lookup"><span data-stu-id="ecbef-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecbef-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecbef-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecbef-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecbef-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecbef-143">Java</span><span class="sxs-lookup"><span data-stu-id="ecbef-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecbef-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecbef-144">Response</span></span>

<span data-ttu-id="ecbef-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ecbef-145">The following is an example of the response.</span></span>
><span data-ttu-id="ecbef-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecbef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
