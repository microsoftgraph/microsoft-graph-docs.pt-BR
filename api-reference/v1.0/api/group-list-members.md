---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais, dispositivos, entidades de serviço e outros grupos como membros.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fce71e0caa13e5b1ba7ac4bf5aab41ecd2e96357
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782550"
---
# <a name="list-members"></a><span data-ttu-id="cea53-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="cea53-104">List members</span></span>

<span data-ttu-id="cea53-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cea53-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cea53-106">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="cea53-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="cea53-107">Um grupo pode ter usuários, contatos organizacionais, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="cea53-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="cea53-108">No momento, as entidades de serviço não estão listadas como membros de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="cea53-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="cea53-109">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="cea53-109">This operation is not transitive.</span></span>

<span data-ttu-id="cea53-110">Quando um grupo contém mais de 100 membros, o Microsoft Graph retorna uma propriedade `@odata.nextLink` na resposta que contém um URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="cea53-110">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="cea53-111">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com o `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph no aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="cea53-111">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="cea53-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="cea53-112">Permissions</span></span>
<span data-ttu-id="cea53-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cea53-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cea53-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cea53-115">Permission type</span></span>      | <span data-ttu-id="cea53-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cea53-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cea53-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cea53-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cea53-118">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cea53-118">User.ReadBasic.All, User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="cea53-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cea53-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cea53-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cea53-120">Not supported.</span></span>    |
|<span data-ttu-id="cea53-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cea53-121">Application</span></span> | <span data-ttu-id="cea53-122">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cea53-122">User.Read.All, GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cea53-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cea53-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cea53-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cea53-124">Optional query parameters</span></span>
<span data-ttu-id="cea53-125">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cea53-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cea53-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cea53-126">Request headers</span></span>
| <span data-ttu-id="cea53-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cea53-127">Header</span></span>       | <span data-ttu-id="cea53-128">Valor</span><span class="sxs-lookup"><span data-stu-id="cea53-128">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cea53-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="cea53-129">Authorization</span></span>  | <span data-ttu-id="cea53-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cea53-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cea53-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cea53-132">Request body</span></span>
<span data-ttu-id="cea53-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cea53-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cea53-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cea53-134">Response</span></span>
<span data-ttu-id="cea53-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cea53-135">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cea53-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cea53-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cea53-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cea53-137">Request</span></span>
<span data-ttu-id="cea53-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cea53-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cea53-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cea53-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="cea53-140">C#</span><span class="sxs-lookup"><span data-stu-id="cea53-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cea53-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cea53-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cea53-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cea53-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cea53-143">Java</span><span class="sxs-lookup"><span data-stu-id="cea53-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cea53-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cea53-144">Response</span></span>
<span data-ttu-id="cea53-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cea53-145">The following is an example of the response.</span></span>
><span data-ttu-id="cea53-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cea53-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

