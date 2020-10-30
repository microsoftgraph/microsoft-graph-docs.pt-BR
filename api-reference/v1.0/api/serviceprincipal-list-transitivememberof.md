---
title: Listar memberOf transitivos de servicePrincipal
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 5d43c8dad7b475f36e8f66a7edc4c22f583c8553
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797078"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="d7019-103">Listar memberOf transitivos de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="d7019-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="d7019-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7019-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7019-105">Obtenha os grupos e funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="d7019-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="d7019-106">Essa operação é transitiva e incluirá todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="d7019-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7019-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7019-107">Permissions</span></span>
<span data-ttu-id="d7019-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7019-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7019-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7019-110">Permission type</span></span>      | <span data-ttu-id="d7019-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7019-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7019-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7019-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7019-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7019-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7019-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7019-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7019-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7019-115">Not supported.</span></span>    |
|<span data-ttu-id="d7019-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7019-116">Application</span></span> | <span data-ttu-id="d7019-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7019-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d7019-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7019-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7019-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d7019-119">Optional query parameters</span></span>

<span data-ttu-id="d7019-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="d7019-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="d7019-121">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="d7019-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="d7019-122">Você pode usar `$search` nas propriedades **displayName** e **descrição** .</span><span class="sxs-lookup"><span data-stu-id="d7019-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="d7019-123">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="d7019-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="d7019-124">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="d7019-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7019-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-125">Request headers</span></span>
| <span data-ttu-id="d7019-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d7019-126">Name</span></span>           | <span data-ttu-id="d7019-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7019-127">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d7019-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7019-128">Authorization</span></span>  | <span data-ttu-id="d7019-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7019-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7019-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="d7019-131">ConsistencyLevel</span></span> | <span data-ttu-id="d7019-132">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="d7019-132">eventual.</span></span> <span data-ttu-id="d7019-133">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="d7019-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="d7019-134">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="d7019-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7019-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-135">Request body</span></span>
<span data-ttu-id="d7019-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7019-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7019-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7019-137">Response</span></span>

<span data-ttu-id="d7019-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7019-138">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7019-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d7019-139">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="d7019-140">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro transitivo</span><span class="sxs-lookup"><span data-stu-id="d7019-140">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="d7019-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-141">Request</span></span>

<span data-ttu-id="d7019-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7019-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf
```

#### <a name="response"></a><span data-ttu-id="d7019-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7019-143">Response</span></span>

<span data-ttu-id="d7019-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7019-144">The following is an example of the response.</span></span> 

> <span data-ttu-id="d7019-145">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d7019-145">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d7019-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7019-146">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="d7019-147">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="d7019-147">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="d7019-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-148">Request</span></span>

<span data-ttu-id="d7019-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7019-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d7019-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7019-150">Response</span></span>

<span data-ttu-id="d7019-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7019-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="d7019-152">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="d7019-152">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="d7019-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-153">Request</span></span>

<span data-ttu-id="d7019-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7019-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d7019-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7019-155">Response</span></span>

<span data-ttu-id="d7019-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7019-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="d7019-157">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d7019-157">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d7019-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-158">Request</span></span>

<span data-ttu-id="d7019-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7019-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d7019-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7019-160">Response</span></span>

<span data-ttu-id="d7019-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7019-161">The following is an example of the response.</span></span>

><span data-ttu-id="d7019-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7019-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="d7019-164">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d7019-164">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d7019-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7019-165">Request</span></span>

<span data-ttu-id="d7019-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7019-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d7019-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7019-167">Response</span></span>

<span data-ttu-id="d7019-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7019-168">The following is an example of the response.</span></span>

><span data-ttu-id="d7019-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7019-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
