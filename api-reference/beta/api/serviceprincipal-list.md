---
title: List servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ec41e5c7d1b673bedda651dab9657515eff5d9db
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290037"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="15a2a-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="15a2a-103">List servicePrincipals</span></span>

<span data-ttu-id="15a2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15a2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15a2a-105">Recupere uma lista de objetos de [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="15a2a-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="15a2a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15a2a-106">Permissions</span></span>

<span data-ttu-id="15a2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15a2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15a2a-109">Permission type</span></span> | <span data-ttu-id="15a2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15a2a-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="15a2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15a2a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15a2a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15a2a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="15a2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15a2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a2a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15a2a-114">Not supported.</span></span> |
| <span data-ttu-id="15a2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15a2a-115">Application</span></span> | <span data-ttu-id="15a2a-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a2a-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15a2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15a2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15a2a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15a2a-118">Optional query parameters</span></span>

<span data-ttu-id="15a2a-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="15a2a-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="15a2a-120">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="15a2a-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="15a2a-121">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="15a2a-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="15a2a-122">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="15a2a-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15a2a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15a2a-123">Request headers</span></span>

| <span data-ttu-id="15a2a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="15a2a-124">Name</span></span> | <span data-ttu-id="15a2a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="15a2a-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="15a2a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="15a2a-126">Authorization</span></span> | <span data-ttu-id="15a2a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15a2a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15a2a-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="15a2a-129">ConsistencyLevel</span></span> | <span data-ttu-id="15a2a-130">ocorra.</span><span class="sxs-lookup"><span data-stu-id="15a2a-130">eventual.</span></span> <span data-ttu-id="15a2a-131">Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="15a2a-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="15a2a-132">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="15a2a-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15a2a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15a2a-133">Request body</span></span>

<span data-ttu-id="15a2a-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15a2a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15a2a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a2a-135">Response</span></span>

<span data-ttu-id="15a2a-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15a2a-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15a2a-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="15a2a-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="15a2a-138">Exemplo 1: obter uma lista de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="15a2a-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="15a2a-139">Solicitar</span><span class="sxs-lookup"><span data-stu-id="15a2a-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/serviceprincipals
```

#### <a name="response"></a><span data-ttu-id="15a2a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a2a-140">Response</span></span>

<span data-ttu-id="15a2a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15a2a-141">The following is an example of the response.</span></span>
><span data-ttu-id="15a2a-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="15a2a-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="15a2a-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15a2a-143">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "displayName":"amasf",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="15a2a-144">Exemplo 2: obter apenas uma contagem de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="15a2a-144">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="15a2a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15a2a-145">Request</span></span>

<span data-ttu-id="15a2a-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15a2a-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="15a2a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a2a-147">Response</span></span>

<span data-ttu-id="15a2a-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15a2a-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="15a2a-149">893</span><span class="sxs-lookup"><span data-stu-id="15a2a-149">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="15a2a-150">Exemplo 3: use $filter e $top para obter uma entidade de serviço com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="15a2a-150">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="15a2a-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15a2a-151">Request</span></span>

<span data-ttu-id="15a2a-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15a2a-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="15a2a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a2a-153">Response</span></span>

<span data-ttu-id="15a2a-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15a2a-154">The following is an example of the response.</span></span>
><span data-ttu-id="15a2a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15a2a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrinciples",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"a",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="15a2a-157">Exemplo 4: Use $search para obter entidades de serviço com nomes de exibição que contenham as letras "equipe", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="15a2a-157">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="15a2a-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15a2a-158">Request</span></span>

<span data-ttu-id="15a2a-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15a2a-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="15a2a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a2a-160">Response</span></span>

<span data-ttu-id="15a2a-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15a2a-161">The following is an example of the response.</span></span>
><span data-ttu-id="15a2a-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15a2a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"myContosoTeam",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
