---
title: Grupo de lista memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro direto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 65132e45aa7b6d4f6d492e2a9f5e5b74194587c5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440425"
---
# <a name="list-group-memberof"></a><span data-ttu-id="94d82-103">Grupo de lista memberOf</span><span class="sxs-lookup"><span data-stu-id="94d82-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d82-104">Obter grupos e unidades administrativas dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="94d82-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="94d82-p101">Essa operação não é transitiva. Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="94d82-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="94d82-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94d82-107">Permissions</span></span>

<span data-ttu-id="94d82-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94d82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94d82-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94d82-110">Permission type</span></span>      | <span data-ttu-id="94d82-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94d82-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94d82-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94d82-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94d82-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94d82-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94d82-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94d82-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94d82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94d82-115">Not supported.</span></span>    |
|<span data-ttu-id="94d82-116">Application</span><span class="sxs-lookup"><span data-stu-id="94d82-116">Application</span></span> | <span data-ttu-id="94d82-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94d82-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94d82-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94d82-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94d82-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94d82-119">Optional query parameters</span></span>
<span data-ttu-id="94d82-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94d82-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94d82-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94d82-121">Request headers</span></span>
| <span data-ttu-id="94d82-122">Nome</span><span class="sxs-lookup"><span data-stu-id="94d82-122">Name</span></span>       | <span data-ttu-id="94d82-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="94d82-123">Type</span></span> | <span data-ttu-id="94d82-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="94d82-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94d82-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="94d82-125">Authorization</span></span>  | <span data-ttu-id="94d82-126">string</span><span class="sxs-lookup"><span data-stu-id="94d82-126">string</span></span>  | <span data-ttu-id="94d82-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94d82-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94d82-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94d82-129">Request body</span></span>
<span data-ttu-id="94d82-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94d82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94d82-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="94d82-131">Response</span></span>
<span data-ttu-id="94d82-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94d82-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94d82-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94d82-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="94d82-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94d82-134">Request</span></span>

<span data-ttu-id="94d82-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94d82-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94d82-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="94d82-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94d82-137">C#</span><span class="sxs-lookup"><span data-stu-id="94d82-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94d82-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="94d82-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94d82-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="94d82-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94d82-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="94d82-140">Response</span></span>

<span data-ttu-id="94d82-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94d82-141">The following is an example of the response.</span></span>
><span data-ttu-id="94d82-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94d82-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94d82-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94d82-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

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
  ]
}
-->
