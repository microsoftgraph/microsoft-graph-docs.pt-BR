---
title: Listar membros transitivos de grupo
description: Obtenha uma lista dos membros do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b713b3fcddbe4d3a7e0b1931847f94c0f1f60692
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082045"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="66211-103">Listar membros transitivos de grupo</span><span class="sxs-lookup"><span data-stu-id="66211-103">List group transitive members</span></span>

<span data-ttu-id="66211-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66211-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66211-105">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="66211-105">Get a list of the group's members.</span></span> <span data-ttu-id="66211-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="66211-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="66211-107">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="66211-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="66211-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="66211-108">Permissions</span></span>

<span data-ttu-id="66211-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66211-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66211-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66211-111">Permission type</span></span> | <span data-ttu-id="66211-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66211-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="66211-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66211-113">Delegated (work or school account)</span></span> | <span data-ttu-id="66211-114">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="66211-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
| <span data-ttu-id="66211-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66211-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66211-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66211-116">Not supported.</span></span> |
| <span data-ttu-id="66211-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66211-117">Application</span></span> | <span data-ttu-id="66211-118">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="66211-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="66211-119">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="66211-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="66211-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66211-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66211-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66211-121">Optional query parameters</span></span>

<span data-ttu-id="66211-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="66211-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="66211-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="66211-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="66211-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="66211-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="66211-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="66211-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66211-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66211-126">Request headers</span></span>

| <span data-ttu-id="66211-127">Nome</span><span class="sxs-lookup"><span data-stu-id="66211-127">Name</span></span> | <span data-ttu-id="66211-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="66211-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="66211-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="66211-129">Authorization</span></span>  | <span data-ttu-id="66211-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66211-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66211-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="66211-132">ConsistencyLevel</span></span> | <span data-ttu-id="66211-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="66211-133">eventual.</span></span> <span data-ttu-id="66211-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="66211-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="66211-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="66211-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66211-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66211-136">Request body</span></span>

<span data-ttu-id="66211-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66211-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66211-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="66211-138">Response</span></span>

<span data-ttu-id="66211-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66211-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66211-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="66211-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="66211-141">Exemplo 1: obter a associação transitiva de um grupo</span><span class="sxs-lookup"><span data-stu-id="66211-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="66211-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66211-142">Request</span></span>

<span data-ttu-id="66211-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66211-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66211-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="66211-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="66211-145">C#</span><span class="sxs-lookup"><span data-stu-id="66211-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66211-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66211-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66211-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66211-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66211-148">Java</span><span class="sxs-lookup"><span data-stu-id="66211-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="66211-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="66211-149">Response</span></span>

<span data-ttu-id="66211-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66211-150">The following is an example of the response.</span></span>

><span data-ttu-id="66211-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66211-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="66211-153">Exemplo 2: obter apenas uma contagem de associação transitiva</span><span class="sxs-lookup"><span data-stu-id="66211-153">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="66211-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66211-154">Request</span></span>

<span data-ttu-id="66211-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66211-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="66211-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="66211-156">Response</span></span>

<span data-ttu-id="66211-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66211-157">The following is an example of the response.</span></span>
><span data-ttu-id="66211-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66211-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="66211-160">893</span><span class="sxs-lookup"><span data-stu-id="66211-160">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="66211-161">Exemplo 3: usar a conversão OData e $search para obter associação em grupos com nomes de exibição que contenham as letras de ' camada ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="66211-161">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="66211-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66211-162">Request</span></span>

<span data-ttu-id="66211-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66211-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="66211-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="66211-164">Response</span></span>

<span data-ttu-id="66211-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66211-165">The following is an example of the response.</span></span>
><span data-ttu-id="66211-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66211-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="66211-168">Exemplo 4: usar o $filter e o elenco OData para obter a associação do usuário em grupos com um nome de exibição que começa com ' A ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="66211-168">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="66211-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66211-169">Request</span></span>

<span data-ttu-id="66211-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66211-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="66211-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="66211-171">Response</span></span>

<span data-ttu-id="66211-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66211-172">The following is an example of the response.</span></span>
><span data-ttu-id="66211-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66211-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


