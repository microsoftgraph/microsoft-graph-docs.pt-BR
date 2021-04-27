---
title: Listar membros transitivos de grupo
description: Obter uma lista dos membros do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7efa264212a8a6dab89b13916ba2971e226e23f8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041362"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="e1b75-103">Listar membros transitivos de grupo</span><span class="sxs-lookup"><span data-stu-id="e1b75-103">List group transitive members</span></span>

<span data-ttu-id="e1b75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b75-105">Obter uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="e1b75-105">Get a list of the group's members.</span></span> <span data-ttu-id="e1b75-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="e1b75-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="e1b75-107">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="e1b75-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1b75-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1b75-108">Permissions</span></span>

<span data-ttu-id="e1b75-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1b75-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1b75-111">Permission type</span></span> | <span data-ttu-id="e1b75-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1b75-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e1b75-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1b75-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b75-114">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1b75-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="e1b75-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1b75-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b75-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1b75-116">Not supported.</span></span> |
| <span data-ttu-id="e1b75-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1b75-117">Application</span></span> | <span data-ttu-id="e1b75-118">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b75-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="e1b75-119">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão Member.Read.Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="e1b75-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e1b75-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b75-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1b75-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1b75-121">Optional query parameters</span></span>

<span data-ttu-id="e1b75-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e1b75-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="e1b75-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e1b75-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="e1b75-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="e1b75-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e1b75-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="e1b75-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1b75-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b75-126">Request headers</span></span>

| <span data-ttu-id="e1b75-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e1b75-127">Name</span></span> | <span data-ttu-id="e1b75-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b75-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e1b75-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1b75-129">Authorization</span></span>  | <span data-ttu-id="e1b75-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1b75-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1b75-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="e1b75-132">ConsistencyLevel</span></span> | <span data-ttu-id="e1b75-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="e1b75-133">eventual.</span></span> <span data-ttu-id="e1b75-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="e1b75-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="e1b75-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="e1b75-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1b75-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b75-136">Request body</span></span>

<span data-ttu-id="e1b75-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1b75-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1b75-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b75-138">Response</span></span>

<span data-ttu-id="e1b75-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b75-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1b75-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e1b75-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="e1b75-141">Exemplo 1: Obter a associação transitiva de um grupo</span><span class="sxs-lookup"><span data-stu-id="e1b75-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="e1b75-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b75-142">Request</span></span>

<span data-ttu-id="e1b75-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b75-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1b75-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b75-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="e1b75-145">C#</span><span class="sxs-lookup"><span data-stu-id="e1b75-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b75-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b75-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b75-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b75-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1b75-148">Java</span><span class="sxs-lookup"><span data-stu-id="e1b75-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e1b75-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b75-149">Response</span></span>

<span data-ttu-id="e1b75-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b75-150">The following is an example of the response.</span></span>

><span data-ttu-id="e1b75-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e1b75-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="e1b75-152">Exemplo 2: Obter apenas uma contagem de associação transitiva</span><span class="sxs-lookup"><span data-stu-id="e1b75-152">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="e1b75-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b75-153">Request</span></span>

<span data-ttu-id="e1b75-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b75-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e1b75-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b75-155">Response</span></span>

<span data-ttu-id="e1b75-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b75-156">The following is an example of the response.</span></span>
><span data-ttu-id="e1b75-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e1b75-157">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="e1b75-158">893</span><span class="sxs-lookup"><span data-stu-id="e1b75-158">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="e1b75-159">Exemplo 3: Use o OData cast e $search para obter associação em grupos com nomes de exibição que contêm as letras "camada" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e1b75-159">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e1b75-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b75-160">Request</span></span>

<span data-ttu-id="e1b75-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b75-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e1b75-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b75-162">Response</span></span>

<span data-ttu-id="e1b75-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b75-163">The following is an example of the response.</span></span>
><span data-ttu-id="e1b75-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e1b75-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="e1b75-165">Exemplo 4: use o OData cast e $filter para obter a associação do usuário em grupos com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e1b75-165">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e1b75-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1b75-166">Request</span></span>

<span data-ttu-id="e1b75-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1b75-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e1b75-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1b75-168">Response</span></span>

<span data-ttu-id="e1b75-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1b75-169">The following is an example of the response.</span></span>
><span data-ttu-id="e1b75-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e1b75-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


