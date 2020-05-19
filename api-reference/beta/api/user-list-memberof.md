---
title: Listar usuário membro
description: Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto. Essa operação não é transitiva.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 81bcfc4ef54037e05390c40ac058466c62bcf9c7
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291024"
---
# <a name="list-user-memberof"></a><span data-ttu-id="ded75-104">Listar usuário membro</span><span class="sxs-lookup"><span data-stu-id="ded75-104">List user memberOf</span></span>

<span data-ttu-id="ded75-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ded75-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ded75-106">Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="ded75-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="ded75-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ded75-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ded75-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ded75-108">Permissions</span></span>

<span data-ttu-id="ded75-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ded75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ded75-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ded75-111">Permission type</span></span> | <span data-ttu-id="ded75-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ded75-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="ded75-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ded75-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ded75-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ded75-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ded75-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ded75-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ded75-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ded75-116">Not supported.</span></span> |
| <span data-ttu-id="ded75-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ded75-117">Application</span></span> | <span data-ttu-id="ded75-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ded75-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ded75-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ded75-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ded75-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ded75-120">Optional query parameters</span></span>

<span data-ttu-id="ded75-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="ded75-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="ded75-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="ded75-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="ded75-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="ded75-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ded75-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="ded75-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ded75-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="ded75-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ded75-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-126">Request headers</span></span>

| <span data-ttu-id="ded75-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ded75-127">Header</span></span> | <span data-ttu-id="ded75-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ded75-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="ded75-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ded75-129">Authorization</span></span>  | <span data-ttu-id="ded75-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ded75-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ded75-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ded75-132">ConsistencyLevel</span></span> | <span data-ttu-id="ded75-133">ocorra.</span><span class="sxs-lookup"><span data-stu-id="ded75-133">eventual.</span></span> <span data-ttu-id="ded75-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="ded75-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="ded75-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="ded75-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ded75-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-136">Request body</span></span>

<span data-ttu-id="ded75-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ded75-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ded75-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded75-138">Response</span></span>

<span data-ttu-id="ded75-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ded75-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ded75-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ded75-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="ded75-141">Exemplo 1: obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="ded75-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="ded75-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-142">Request</span></span>

<span data-ttu-id="ded75-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded75-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="ded75-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded75-144">Response</span></span>

<span data-ttu-id="ded75-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ded75-145">The following is an example of the response.</span></span>
><span data-ttu-id="ded75-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ded75-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ded75-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ded75-147">All the properties will be returned from an actual call.</span></span>

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
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="ded75-148">Exemplo 2: obter apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="ded75-148">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="ded75-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-149">Request</span></span>

<span data-ttu-id="ded75-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded75-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ded75-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded75-151">Response</span></span>

<span data-ttu-id="ded75-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ded75-152">The following is an example of the response.</span></span>
><span data-ttu-id="ded75-153">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ded75-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ded75-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ded75-154">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="ded75-155">893</span><span class="sxs-lookup"><span data-stu-id="ded75-155">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="ded75-156">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="ded75-156">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="ded75-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-157">Request</span></span>

<span data-ttu-id="ded75-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded75-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ded75-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded75-159">Response</span></span>

<span data-ttu-id="ded75-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ded75-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="ded75-161">294</span><span class="sxs-lookup"><span data-stu-id="ded75-161">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="ded75-162">Exemplo 4: Use $search e a conversão OData para obter associação em grupos com nomes de exibição que contenham as letras "Tier", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ded75-162">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ded75-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-163">Request</span></span>

<span data-ttu-id="ded75-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded75-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ded75-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded75-165">Response</span></span>

<span data-ttu-id="ded75-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ded75-166">The following is an example of the response.</span></span>
><span data-ttu-id="ded75-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ded75-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ded75-169">Exemplo 5: use $filter e a conversão OData para obter grupos com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ded75-169">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ded75-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ded75-170">Request</span></span>

<span data-ttu-id="ded75-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded75-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ded75-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ded75-172">Response</span></span>

<span data-ttu-id="ded75-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ded75-173">The following is an example of the response.</span></span>
><span data-ttu-id="ded75-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ded75-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
