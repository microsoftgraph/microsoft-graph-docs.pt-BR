---
title: Listar membros transitivos de grupo
description: Obter uma lista dos membros do grupo. Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros. Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4795eea214654bf482dd053739f8415e890ff2fa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052289"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="a1e43-105">Listar membros transitivos de grupo</span><span class="sxs-lookup"><span data-stu-id="a1e43-105">List group transitive members</span></span>

<span data-ttu-id="a1e43-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1e43-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1e43-107">Obter uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1e43-107">Get a list of the group's members.</span></span> <span data-ttu-id="a1e43-108">Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="a1e43-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="a1e43-109">Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="a1e43-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1e43-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1e43-110">Permissions</span></span>

<span data-ttu-id="a1e43-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1e43-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e43-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1e43-113">Permission type</span></span>      | <span data-ttu-id="a1e43-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1e43-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1e43-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1e43-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a1e43-116">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1e43-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="a1e43-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1e43-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1e43-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1e43-118">Not supported.</span></span>    |
|<span data-ttu-id="a1e43-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1e43-119">Application</span></span> | <span data-ttu-id="a1e43-120">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1e43-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

><span data-ttu-id="a1e43-121">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão Member.Read.Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="a1e43-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a1e43-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e43-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1e43-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1e43-123">Optional query parameters</span></span>

<span data-ttu-id="a1e43-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a1e43-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a1e43-125">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="a1e43-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="a1e43-126">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="a1e43-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a1e43-127">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="a1e43-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1e43-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e43-128">Request headers</span></span>

| <span data-ttu-id="a1e43-129">Nome</span><span class="sxs-lookup"><span data-stu-id="a1e43-129">Name</span></span> | <span data-ttu-id="a1e43-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e43-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="a1e43-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1e43-131">Authorization</span></span>  | <span data-ttu-id="a1e43-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1e43-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1e43-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a1e43-134">ConsistencyLevel</span></span> | <span data-ttu-id="a1e43-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="a1e43-135">eventual.</span></span> <span data-ttu-id="a1e43-136">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="a1e43-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a1e43-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="a1e43-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1e43-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e43-138">Request body</span></span>

<span data-ttu-id="a1e43-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1e43-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1e43-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e43-140">Response</span></span>

<span data-ttu-id="a1e43-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e43-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1e43-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1e43-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="a1e43-143">Exemplo 1: Obter a associação transitiva de um grupo</span><span class="sxs-lookup"><span data-stu-id="a1e43-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="a1e43-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e43-144">Request</span></span>

<span data-ttu-id="a1e43-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e43-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1e43-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e43-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="a1e43-147">C#</span><span class="sxs-lookup"><span data-stu-id="a1e43-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1e43-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1e43-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1e43-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1e43-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1e43-150">Java</span><span class="sxs-lookup"><span data-stu-id="a1e43-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a1e43-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e43-151">Response</span></span>

<span data-ttu-id="a1e43-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e43-152">The following is an example of the response.</span></span>

><span data-ttu-id="a1e43-153">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1e43-153">**Note**: The response object shown here might be shortened for readability.</span></span>

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
      "@odata.type": "#microsoft.graph.user",
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="a1e43-154">Exemplo 2: Obter apenas uma contagem de associação transitiva</span><span class="sxs-lookup"><span data-stu-id="a1e43-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="a1e43-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e43-155">Request</span></span>

<span data-ttu-id="a1e43-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e43-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a1e43-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e43-157">Response</span></span>

<span data-ttu-id="a1e43-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e43-158">The following is an example of the response.</span></span>

><span data-ttu-id="a1e43-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1e43-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="a1e43-160">Exemplo 3: Use o OData cast e $search para obter associação em grupos com nomes de exibição que contêm as letras "camada" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a1e43-160">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a1e43-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e43-161">Request</span></span>

<span data-ttu-id="a1e43-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e43-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a1e43-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e43-163">Response</span></span>

<span data-ttu-id="a1e43-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e43-164">The following is an example of the response.</span></span>

><span data-ttu-id="a1e43-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1e43-165">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a1e43-166">Exemplo 4: use o OData cast e $filter para obter a associação do usuário em grupos com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a1e43-166">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a1e43-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e43-167">Request</span></span>

<span data-ttu-id="a1e43-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e43-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a1e43-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e43-169">Response</span></span>

<span data-ttu-id="a1e43-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e43-170">The following is an example of the response.</span></span>

><span data-ttu-id="a1e43-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1e43-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
