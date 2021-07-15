---
title: Listar grupos
description: Liste todos os grupos disponíveis em uma organização, incluindo, entre outros, os grupos do Microsoft 365.
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bc3415ab5bc2610341a6f5c9645cc93b2defbee2
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430169"
---
# <a name="list-groups"></a><span data-ttu-id="31900-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="31900-103">List groups</span></span>

<span data-ttu-id="31900-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31900-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31900-105">Liste todos os grupos em uma organização, incluindo, entre outros, os grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="31900-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="31900-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="31900-106">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="31900-107">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="31900-107">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="31900-108">Para obter propriedades _não_ retornadas por padrão, execute uma operação [GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="31900-108">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="31900-109">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="31900-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="31900-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="31900-110">Permissions</span></span>
<span data-ttu-id="31900-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31900-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31900-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31900-113">Permission type</span></span>      | <span data-ttu-id="31900-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31900-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31900-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31900-115">Delegated (work or school account)</span></span> | <span data-ttu-id="31900-116">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="31900-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="31900-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31900-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31900-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31900-118">Not supported.</span></span>    |
|<span data-ttu-id="31900-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31900-119">Application</span></span> | <span data-ttu-id="31900-120">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="31900-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31900-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31900-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31900-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="31900-122">Optional query parameters</span></span>
<span data-ttu-id="31900-123">Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-123">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="31900-124">Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`.</span><span class="sxs-lookup"><span data-stu-id="31900-124">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="31900-125">Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-125">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<span data-ttu-id="31900-126">Para listar apenas grupos do Microsoft 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="31900-126">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="31900-127">O `$search` parâmetro de consulta suporta a tokenização apenas nos campos **displayName** e **description** e requer o cabeçalho **ConsistencyLevel**.</span><span class="sxs-lookup"><span data-stu-id="31900-127">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields and requires the **ConsistencyLevel** header.</span></span> <span data-ttu-id="31900-128">Qualquer campo além de **displayName** e **description** é padrão para o comportamento`$filter``startswith`.</span><span class="sxs-lookup"><span data-stu-id="31900-128">Fields other than **displayName** and **description** default to `$filter` `startswith` behavior.</span></span>

<span data-ttu-id="31900-129">Para obter mais informações sobre as opções de consulta OData, veja [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="31900-129">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="31900-130">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-130">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31900-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-131">Request headers</span></span>

| <span data-ttu-id="31900-132">Nome</span><span class="sxs-lookup"><span data-stu-id="31900-132">Name</span></span> | <span data-ttu-id="31900-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="31900-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="31900-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="31900-134">Authorization</span></span>  | <span data-ttu-id="31900-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31900-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31900-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="31900-137">ConsistencyLevel</span></span> | <span data-ttu-id="31900-138">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="31900-138">eventual.</span></span> <span data-ttu-id="31900-139">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`.</span><span class="sxs-lookup"><span data-stu-id="31900-139">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="31900-140">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-140">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="31900-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-141">Request body</span></span>
<span data-ttu-id="31900-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31900-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31900-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-143">Response</span></span>
<span data-ttu-id="31900-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="31900-145">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="31900-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="31900-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31900-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="31900-147">Exemplo 1: Obter uma lista de grupos</span><span class="sxs-lookup"><span data-stu-id="31900-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="31900-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-148">Request</span></span>

<span data-ttu-id="31900-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31900-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="31900-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```
# <a name="c"></a>[<span data-ttu-id="31900-151">C#</span><span class="sxs-lookup"><span data-stu-id="31900-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31900-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31900-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31900-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31900-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31900-154">Java</span><span class="sxs-lookup"><span data-stu-id="31900-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31900-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-155">Response</span></span>

<span data-ttu-id="31900-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-156">The following is an example of the response.</span></span>

><span data-ttu-id="31900-p109">**Observação:** o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31900-p109">**Note:** The response object shown here might be shortened for readability. All the default properties are returned for each group in an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T02:21:05Z",
      "description": "Self help community for golf",
      "displayName": "Golf Assist",
      "expirationDateTime": null,
      "groupTypes": [
        "Unified"
      ],
      "isAssignableToRole": null,
      "mail": "golfassist@contoso.com",
      "mailEnabled": true,
      "mailNickname": "golfassist",
      "membershipRule": null,
      "membershipRuleProcessingState": null,
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "preferredLanguage": null,
      "proxyAddresses": [
        "smtp:golfassist@contoso.onmicrosoft.com",
        "SMTP:golfassist@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T02:21:05Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "theme": null,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
    },
    {
      "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-11-19T20:29:40Z",
      "description": "Talk about golf",
      "displayName": "Golf Discussion",
      "expirationDateTime": null,
      "groupTypes": [],
      "isAssignableToRole": null,
      "mail": "golftalk@contoso.com",
      "mailEnabled": true,
      "mailNickname": "golftalk",
      "membershipRule": null,
      "membershipRuleProcessingState": null,
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "preferredLanguage": null,
      "proxyAddresses": [
        "smtp:golftalk@contoso.onmicrosoft.com",
        "SMTP:golftalk@contoso.com"
      ],
      "renewedDateTime": "2018-11-19T20:29:40Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "theme": null,
      "visibility": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="31900-159">Exemplo 2: Obter uma lista filtrada de grupos, incluindo a contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="31900-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

<span data-ttu-id="31900-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-160">The following is an example of the request.</span></span> <span data-ttu-id="31900-161">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-161">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="31900-162">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-162">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

#### <a name="request"></a><span data-ttu-id="31900-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-163">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="31900-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-164">Response</span></span>

<span data-ttu-id="31900-165">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="31900-165">The following is an example of the response which includes only the requested properties.</span></span>

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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
   "@odata.count":2,
   "value":[
      {
         "id":"11111111-2222-3333-4444-555555555555",
         "displayName":"Contoso Group 1"
      },
      {
         "id":"22222222-3333-4444-5555-666666666666",
         "displayName":"Contoso Group 2"
      }
   ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="31900-166">Exemplo 3: Obter apenas uma contagem de grupos</span><span class="sxs-lookup"><span data-stu-id="31900-166">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="31900-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-167">Request</span></span>

<span data-ttu-id="31900-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-168">The following is an example of the request.</span></span> <span data-ttu-id="31900-169">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-169">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="31900-170">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-170">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
  }-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="31900-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-171">Response</span></span>

<span data-ttu-id="31900-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="31900-173">Exemplo 4: Utilize $filter e $top para obter um grupo com um nome de exibição que comece com 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="31900-173">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="31900-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-174">Request</span></span>

<span data-ttu-id="31900-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-175">The following is an example of the request.</span></span> <span data-ttu-id="31900-176">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="31900-176">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="31900-177">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-177">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="31900-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-178">Response</span></span>

<span data-ttu-id="31900-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-179">The following is an example of the response.</span></span>

><span data-ttu-id="31900-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31900-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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
   "@odata.count":1,
   "value":[
      {
         "displayName":"a",
         "mailNickname":"a241"
      }
   ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="31900-181">Exemplo 5: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="31900-181">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="31900-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-182">Request</span></span>

<span data-ttu-id="31900-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-183">The following is an example of the request.</span></span> <span data-ttu-id="31900-184">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-184">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="31900-185">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-185">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="31900-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-186">Response</span></span>

<span data-ttu-id="31900-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-187">The following is an example of the response.</span></span>

><span data-ttu-id="31900-188">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31900-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
   "@odata.count":1396,
   "value":[
      {
         "displayName":"SFA Videos",
         "mail":"SFAVideos@service.contoso.com",
         "mailNickname":"SFAVideos"
      }
   ]
}
```

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="31900-189">Exemplo 6: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo' ou uma descrição que contenha as letras 'prod', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="31900-189">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="31900-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31900-190">Request</span></span>

<span data-ttu-id="31900-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-191">The following is an example of the request.</span></span> <span data-ttu-id="31900-192">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="31900-192">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="31900-193">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="31900-193">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="31900-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="31900-194">Response</span></span>

<span data-ttu-id="31900-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31900-195">The following is an example of the response.</span></span>

><span data-ttu-id="31900-196">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31900-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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
   "@odata.count":1396,
   "value":[
      {
         "displayName":"SFA Videos",
         "mail":"SFAVideos@service.contoso.com",
         "mailNickname":"SFAVideos"
      },
      {
         "description":"Video Production",
         "displayName":"Video Production",
         "mail":"videoprod@service.contoso.com",
         "mailNickname":"VideoProduction"
      }
   ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

