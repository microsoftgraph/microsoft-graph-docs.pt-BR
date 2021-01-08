---
title: Listar grupos
description: Liste todos os grupos disponíveis em uma organização, incluindo, entre outros, os grupos do Microsoft 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5a9d138ac1280d419a9a6c386c8f4987d56ac946
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784812"
---
# <a name="list-groups"></a><span data-ttu-id="43f81-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="43f81-103">List groups</span></span>

<span data-ttu-id="43f81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43f81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f81-105">Liste todos os grupos em uma organização, incluindo, entre outros, os grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="43f81-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="43f81-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="43f81-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="43f81-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="43f81-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="43f81-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="43f81-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="43f81-109">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="43f81-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="43f81-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="43f81-110">Permissions</span></span>

<span data-ttu-id="43f81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43f81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43f81-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43f81-113">Permission type</span></span> | <span data-ttu-id="43f81-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43f81-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="43f81-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43f81-115">Delegated (work or school account)</span></span> | <span data-ttu-id="43f81-116">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="43f81-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="43f81-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43f81-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43f81-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43f81-118">Not supported.</span></span> |
| <span data-ttu-id="43f81-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f81-119">Application</span></span> | <span data-ttu-id="43f81-120">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="43f81-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43f81-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43f81-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43f81-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43f81-122">Optional query parameters</span></span>

<span data-ttu-id="43f81-123">Para listar apenas grupos do Microsoft 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="43f81-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="43f81-124">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="43f81-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="43f81-125">Você também pode usar os `$count` e `$search` parâmetros de consulta para limitar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="43f81-126">O `$search` parâmetro de consulta suporta a tokenização apenas nos campos **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="43f81-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="43f81-127">Outros campos são padrão para o `$filter` comportamento.</span><span class="sxs-lookup"><span data-stu-id="43f81-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="43f81-128">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="43f81-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="43f81-129">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="43f81-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="43f81-130">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="43f81-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43f81-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-131">Request headers</span></span>

| <span data-ttu-id="43f81-132">Nome</span><span class="sxs-lookup"><span data-stu-id="43f81-132">Name</span></span> | <span data-ttu-id="43f81-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f81-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="43f81-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="43f81-134">Authorization</span></span>  | <span data-ttu-id="43f81-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43f81-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43f81-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="43f81-137">ConsistencyLevel</span></span> | <span data-ttu-id="43f81-138">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="43f81-138">eventual.</span></span> <span data-ttu-id="43f81-139">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="43f81-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="43f81-140">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="43f81-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43f81-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-141">Request body</span></span>

<span data-ttu-id="43f81-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43f81-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43f81-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-143">Response</span></span>

<span data-ttu-id="43f81-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="43f81-145">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="43f81-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="43f81-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43f81-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="43f81-147">Exemplo 1: Obter uma lista de grupos</span><span class="sxs-lookup"><span data-stu-id="43f81-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-148">Request</span></span>

<span data-ttu-id="43f81-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f81-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43f81-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="43f81-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="43f81-151">C#</span><span class="sxs-lookup"><span data-stu-id="43f81-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43f81-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43f81-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43f81-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43f81-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43f81-154">Java</span><span class="sxs-lookup"><span data-stu-id="43f81-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="43f81-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-155">Response</span></span>

<span data-ttu-id="43f81-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-156">The following is an example of the response.</span></span>
><span data-ttu-id="43f81-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="43f81-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="43f81-158">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43f81-158">All the default properties are returned for each group in an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
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

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="43f81-159">Exemplo 2: Obter uma lista filtrada de grupos, incluindo a contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="43f81-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="43f81-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-161">Response</span></span>

<span data-ttu-id="43f81-162">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="43f81-162">The following is an example of the response which includes only the requested properties.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
  "@odata.count":2,
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "displayName": "Contoso Group 1"
    },
    {
      "id": "22222222-3333-4444-5555-666666666666",
      "displayName": "Contoso Group 2"
    }
  ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="43f81-163">Exemplo 3: Obter apenas uma contagem de grupos</span><span class="sxs-lookup"><span data-stu-id="43f81-163">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-164">Request</span></span>

<span data-ttu-id="43f81-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f81-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="43f81-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-166">Response</span></span>

<span data-ttu-id="43f81-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-167">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="43f81-168">893</span><span class="sxs-lookup"><span data-stu-id="43f81-168">893</span></span>


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="43f81-169">Exemplo 4: Utilize $filter e $top para obter um grupo com um nome de exibição que comece com 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="43f81-169">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-170">Request</span></span>

<span data-ttu-id="43f81-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f81-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="43f81-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-172">Response</span></span>

<span data-ttu-id="43f81-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-173">The following is an example of the response.</span></span>
><span data-ttu-id="43f81-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43f81-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mailNickname":"a241"
    }
  ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="43f81-176">Exemplo 5: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="43f81-176">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-177">Request</span></span>

<span data-ttu-id="43f81-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f81-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="43f81-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-179">Response</span></span>

<span data-ttu-id="43f81-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-180">The following is an example of the response.</span></span>
><span data-ttu-id="43f81-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43f81-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="43f81-183">Exemplo 6: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo' ou uma descrição que contenha as letras 'prod', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="43f81-183">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-184">Request</span></span>

<span data-ttu-id="43f81-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f81-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="43f81-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-186">Response</span></span>

<span data-ttu-id="43f81-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-187">The following is an example of the response.</span></span>
><span data-ttu-id="43f81-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43f81-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-7-list-dynamic-groups-filtered-by-enabled-membershipruleprocessingstate"></a><span data-ttu-id="43f81-190">Exemplo 7: Listar grupos dinâmicos, filtrados por MembershipRuleProcessingState habilitado</span><span class="sxs-lookup"><span data-stu-id="43f81-190">Example 7: List dynamic groups, filtered by enabled membershipRuleProcessingState</span></span>

#### <a name="request"></a><span data-ttu-id="43f81-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f81-191">Request</span></span>

<span data-ttu-id="43f81-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f81-192">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_enabled_dynamic_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus&$filter=membershipRuleProcessingState eq 'On'
```

#### <a name="response"></a><span data-ttu-id="43f81-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f81-193">Response</span></span>

<span data-ttu-id="43f81-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f81-194">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus)",
  "value":[
    {
      "id": "1cdf9c18-a7dc-46b1-b47f-094d5656376d",
      "membershipRule": "user.accountEnabled -eq false",
      "membershipRuleProcessingState": "On",
      "membershipRuleProcessingStatus": {
          "status" : "Succeeded",
          "lastMembershipUpdated"  : "2020-09-14T00:00:00Z",
          "errorMessage" : null
        }
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


