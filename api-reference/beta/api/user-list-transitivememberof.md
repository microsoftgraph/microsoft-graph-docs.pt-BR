---
title: Listar usuário transitivo memberOf
description: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro. Essa solicitação de API é transitiva e também retornará todos os grupos de que o usuário é membro aninhado.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 20d2a8b0384a3c346a0f1f3f9f1a8b66cd9a6bfa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720722"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="88197-104">Listar usuário transitivo memberOf</span><span class="sxs-lookup"><span data-stu-id="88197-104">List user transitive memberOf</span></span>

<span data-ttu-id="88197-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88197-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88197-106">Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="88197-106">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="88197-107">Essa solicitação de API é transitiva e também retornará todos os grupos de que o usuário é membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="88197-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="88197-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="88197-108">Permissions</span></span>

<span data-ttu-id="88197-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88197-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88197-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88197-111">Permission type</span></span> | <span data-ttu-id="88197-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88197-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="88197-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88197-113">Delegated (work or school account)</span></span> | <span data-ttu-id="88197-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88197-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="88197-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88197-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88197-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88197-116">Not supported.</span></span> |
| <span data-ttu-id="88197-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88197-117">Application</span></span> | <span data-ttu-id="88197-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88197-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88197-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88197-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88197-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88197-120">Optional query parameters</span></span>

<span data-ttu-id="88197-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="88197-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="88197-122">O OData cast também está habilitado, por exemplo, você pode lançar para obter apenas a associação transitiva em grupos.</span><span class="sxs-lookup"><span data-stu-id="88197-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="88197-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="88197-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="88197-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="88197-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="88197-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="88197-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88197-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-126">Request headers</span></span>

| <span data-ttu-id="88197-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88197-127">Header</span></span> | <span data-ttu-id="88197-128">Valor</span><span class="sxs-lookup"><span data-stu-id="88197-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="88197-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="88197-129">Authorization</span></span>  | <span data-ttu-id="88197-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88197-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88197-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="88197-132">ConsistencyLevel</span></span> | <span data-ttu-id="88197-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="88197-133">eventual.</span></span> <span data-ttu-id="88197-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="88197-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="88197-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="88197-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88197-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-136">Request body</span></span>

<span data-ttu-id="88197-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88197-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88197-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="88197-138">Response</span></span>

<span data-ttu-id="88197-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88197-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88197-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="88197-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="88197-141">Exemplo 1: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro</span><span class="sxs-lookup"><span data-stu-id="88197-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="88197-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-142">Request</span></span>

<span data-ttu-id="88197-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88197-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="88197-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="88197-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="88197-145">C#</span><span class="sxs-lookup"><span data-stu-id="88197-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88197-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88197-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88197-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88197-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88197-148">Java</span><span class="sxs-lookup"><span data-stu-id="88197-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="88197-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="88197-149">Response</span></span>

<span data-ttu-id="88197-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88197-150">The following is an example of the response.</span></span>
><span data-ttu-id="88197-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88197-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"ContosoAudience_PugetSound",
      "mailEnabled":true,
      "mailNickname":"Contoso_PugetSound",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="88197-153">Exemplo 2: Obter apenas uma contagem de associação transitiva em grupos, funções de diretório e unidades administrativas</span><span class="sxs-lookup"><span data-stu-id="88197-153">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="88197-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-154">Request</span></span>

<span data-ttu-id="88197-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88197-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="88197-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="88197-156">Response</span></span>

<span data-ttu-id="88197-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88197-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="88197-158">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="88197-158">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="88197-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-159">Request</span></span>

<span data-ttu-id="88197-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88197-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="88197-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="88197-161">Response</span></span>

<span data-ttu-id="88197-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88197-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

588
```

### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="88197-163">Exemplo 4: use $search e OData cast para obter associação transitiva em grupos com nomes de exibição que contêm as letras 'camada' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="88197-163">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="88197-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-164">Request</span></span>

<span data-ttu-id="88197-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88197-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="88197-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="88197-166">Response</span></span>

<span data-ttu-id="88197-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88197-167">The following is an example of the response.</span></span>
><span data-ttu-id="88197-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88197-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="88197-170">Exemplo 5: use $filter e OData cast para obter associação transitiva em grupos com um nome de exibição que começa com "a" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="88197-170">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="88197-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88197-171">Request</span></span>

<span data-ttu-id="88197-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88197-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="88197-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="88197-173">Response</span></span>

<span data-ttu-id="88197-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88197-174">The following is an example of the response.</span></span>
><span data-ttu-id="88197-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88197-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


