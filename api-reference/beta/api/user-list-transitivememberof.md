---
title: Listar usuário transitiva membro
description: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e30ffe72da624cc6ce304e9775f933969b2c9659
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290624"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="04720-104">Listar usuário transitiva membro</span><span class="sxs-lookup"><span data-stu-id="04720-104">List user transitive memberOf</span></span>

<span data-ttu-id="04720-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04720-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04720-106">Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="04720-106">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="04720-107">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="04720-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="04720-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="04720-108">Permissions</span></span>

<span data-ttu-id="04720-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04720-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04720-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04720-111">Permission type</span></span> | <span data-ttu-id="04720-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04720-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="04720-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04720-113">Delegated (work or school account)</span></span> | <span data-ttu-id="04720-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04720-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="04720-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04720-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04720-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04720-116">Not supported.</span></span> |
| <span data-ttu-id="04720-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04720-117">Application</span></span> | <span data-ttu-id="04720-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04720-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04720-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04720-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04720-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04720-120">Optional query parameters</span></span>

<span data-ttu-id="04720-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="04720-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="04720-122">O elenco do OData também é habilitado, por exemplo, você pode transmitir para obter apenas a associação transitiva em grupos.</span><span class="sxs-lookup"><span data-stu-id="04720-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="04720-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="04720-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="04720-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="04720-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="04720-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="04720-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04720-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-126">Request headers</span></span>

| <span data-ttu-id="04720-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04720-127">Header</span></span> | <span data-ttu-id="04720-128">Valor</span><span class="sxs-lookup"><span data-stu-id="04720-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="04720-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="04720-129">Authorization</span></span>  | <span data-ttu-id="04720-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04720-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04720-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="04720-132">ConsistencyLevel</span></span> | <span data-ttu-id="04720-133">ocorra.</span><span class="sxs-lookup"><span data-stu-id="04720-133">eventual.</span></span> <span data-ttu-id="04720-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="04720-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="04720-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="04720-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04720-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-136">Request body</span></span>

<span data-ttu-id="04720-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04720-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04720-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="04720-138">Response</span></span>

<span data-ttu-id="04720-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04720-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04720-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04720-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="04720-141">Exemplo 1: obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro</span><span class="sxs-lookup"><span data-stu-id="04720-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="04720-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-142">Request</span></span>

<span data-ttu-id="04720-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04720-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf
```

#### <a name="response"></a><span data-ttu-id="04720-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="04720-144">Response</span></span>

<span data-ttu-id="04720-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04720-145">The following is an example of the response.</span></span>
><span data-ttu-id="04720-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="04720-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04720-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04720-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="04720-148">Exemplo 2: obter apenas uma contagem de associação transitiva em grupos, funções de diretório e unidades administrativas</span><span class="sxs-lookup"><span data-stu-id="04720-148">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="04720-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-149">Request</span></span>

<span data-ttu-id="04720-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04720-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="04720-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="04720-151">Response</span></span>

<span data-ttu-id="04720-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04720-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="04720-153">893</span><span class="sxs-lookup"><span data-stu-id="04720-153">893</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="04720-154">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="04720-154">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="04720-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-155">Request</span></span>

<span data-ttu-id="04720-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04720-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="04720-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="04720-157">Response</span></span>

<span data-ttu-id="04720-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04720-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="04720-159">588</span><span class="sxs-lookup"><span data-stu-id="04720-159">588</span></span>


### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="04720-160">Exemplo 4: Use $search e a conversão OData para obter uma associação transitiva em grupos com nomes de exibição que contenham as letras "Tier", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="04720-160">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="04720-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-161">Request</span></span>

<span data-ttu-id="04720-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04720-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="04720-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="04720-163">Response</span></span>

<span data-ttu-id="04720-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04720-164">The following is an example of the response.</span></span>
><span data-ttu-id="04720-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04720-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="04720-167">Exemplo 5: use $filter e o elenco OData para obter uma associação transitiva em grupos com um nome de exibição que começa com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="04720-167">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="04720-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04720-168">Request</span></span>

<span data-ttu-id="04720-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04720-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="04720-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="04720-170">Response</span></span>

<span data-ttu-id="04720-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04720-171">The following is an example of the response.</span></span>
><span data-ttu-id="04720-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04720-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
