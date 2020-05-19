---
title: Listar o servicePrincipalName memberOf
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 31f40cc2abd804d29e63f7532542657a4d268d16
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291220"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="01179-104">Listar o servicePrincipalName memberOf</span><span class="sxs-lookup"><span data-stu-id="01179-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="01179-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01179-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01179-106">Obtenha os grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="01179-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="01179-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="01179-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="01179-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="01179-108">Permissions</span></span>

<span data-ttu-id="01179-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01179-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01179-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01179-111">Permission type</span></span>      | <span data-ttu-id="01179-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01179-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01179-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01179-113">Delegated (work or school account)</span></span> | <span data-ttu-id="01179-114">Application. Read. All, Directory. Read. All, Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="01179-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01179-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01179-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01179-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01179-116">Not supported.</span></span>    |
|<span data-ttu-id="01179-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01179-117">Application</span></span> | <span data-ttu-id="01179-118">Application. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="01179-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="01179-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01179-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01179-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01179-120">Optional query parameters</span></span>

<span data-ttu-id="01179-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="01179-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="01179-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="01179-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="01179-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="01179-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="01179-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="01179-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="01179-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="01179-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01179-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-126">Request headers</span></span>

| <span data-ttu-id="01179-127">Nome</span><span class="sxs-lookup"><span data-stu-id="01179-127">Name</span></span>       | <span data-ttu-id="01179-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="01179-128">Type</span></span> | <span data-ttu-id="01179-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="01179-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01179-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="01179-130">Authorization</span></span>  | <span data-ttu-id="01179-131">string</span><span class="sxs-lookup"><span data-stu-id="01179-131">string</span></span>  | <span data-ttu-id="01179-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01179-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01179-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="01179-134">ConsistencyLevel</span></span> | <span data-ttu-id="01179-135">ocorra.</span><span class="sxs-lookup"><span data-stu-id="01179-135">eventual.</span></span> <span data-ttu-id="01179-136">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="01179-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="01179-137">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="01179-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01179-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-138">Request body</span></span>
<span data-ttu-id="01179-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01179-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01179-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="01179-140">Response</span></span>

<span data-ttu-id="01179-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01179-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01179-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="01179-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="01179-143">Exemplo 1: obter grupos e funções de diretório de que a entidade de serviço é um membro direto de</span><span class="sxs-lookup"><span data-stu-id="01179-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="01179-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-144">Request</span></span>

<span data-ttu-id="01179-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01179-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="01179-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="01179-146">Response</span></span>

<span data-ttu-id="01179-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01179-147">The following is an example of the response.</span></span> 
> <span data-ttu-id="01179-148">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="01179-148">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="01179-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01179-149">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="01179-150">Exemplo 2: obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="01179-150">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="01179-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-151">Request</span></span>

<span data-ttu-id="01179-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01179-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01179-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="01179-153">Response</span></span>

<span data-ttu-id="01179-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01179-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="01179-155">394</span><span class="sxs-lookup"><span data-stu-id="01179-155">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="01179-156">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="01179-156">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="01179-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-157">Request</span></span>

<span data-ttu-id="01179-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01179-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01179-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="01179-159">Response</span></span>

<span data-ttu-id="01179-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01179-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="01179-161">394</span><span class="sxs-lookup"><span data-stu-id="01179-161">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="01179-162">Exemplo 4: Use $search e a conversão OData para obter Associação de grupo com nomes de exibição que contenham as letras "vídeo", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="01179-162">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="01179-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-163">Request</span></span>

<span data-ttu-id="01179-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01179-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01179-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="01179-165">Response</span></span>

<span data-ttu-id="01179-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01179-166">The following is an example of the response.</span></span>
><span data-ttu-id="01179-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01179-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1396,
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="01179-169">Exemplo 5: use $filter e a conversão OData para obter a associação de grupo com um nome de exibição que comece com a letra "A", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="01179-169">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="01179-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01179-170">Request</span></span>

<span data-ttu-id="01179-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01179-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01179-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="01179-172">Response</span></span>

<span data-ttu-id="01179-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01179-173">The following is an example of the response.</span></span>
><span data-ttu-id="01179-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01179-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":76,
  "value":[
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
