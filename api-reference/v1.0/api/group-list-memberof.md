---
title: Listar memberOf
description: 'Obtenha grupos dos quais um grupo é um membro direto. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 120cb02837ee30bc67ce315e158d4d4361a8be42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517072"
---
# <a name="list-memberof"></a><span data-ttu-id="6d930-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="6d930-103">List memberOf</span></span>

<span data-ttu-id="6d930-104">Namespace: microsoft.graph Obtenha os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="6d930-104">Namespace: microsoft.graph Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="6d930-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="6d930-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d930-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d930-107">Permissions</span></span>
<span data-ttu-id="6d930-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d930-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d930-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d930-110">Permission type</span></span>      | <span data-ttu-id="6d930-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d930-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d930-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d930-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d930-113">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d930-113">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="6d930-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d930-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d930-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d930-115">Not supported.</span></span>    |
|<span data-ttu-id="6d930-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d930-116">Application</span></span> | <span data-ttu-id="6d930-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d930-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6d930-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d930-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d930-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d930-119">Optional query parameters</span></span>
<span data-ttu-id="6d930-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d930-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d930-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d930-121">Request headers</span></span>
| <span data-ttu-id="6d930-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6d930-122">Name</span></span>       | <span data-ttu-id="6d930-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d930-123">Type</span></span> | <span data-ttu-id="6d930-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d930-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d930-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d930-125">Authorization</span></span>  | <span data-ttu-id="6d930-126">string</span><span class="sxs-lookup"><span data-stu-id="6d930-126">string</span></span>  | <span data-ttu-id="6d930-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d930-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d930-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d930-129">Request body</span></span>
<span data-ttu-id="6d930-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d930-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d930-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d930-131">Response</span></span>
<span data-ttu-id="6d930-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d930-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d930-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d930-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6d930-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d930-134">Request</span></span>
<span data-ttu-id="6d930-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d930-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d930-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d930-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="6d930-137">C#</span><span class="sxs-lookup"><span data-stu-id="6d930-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d930-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d930-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d930-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d930-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d930-140">Java</span><span class="sxs-lookup"><span data-stu-id="6d930-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6d930-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d930-141">Response</span></span>
<span data-ttu-id="6d930-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d930-142">The following is an example of the response.</span></span>
><span data-ttu-id="6d930-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6d930-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d930-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d930-144">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
