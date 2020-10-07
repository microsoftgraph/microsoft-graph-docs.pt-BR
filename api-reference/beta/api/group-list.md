---
title: Listar grupos
description: Liste todos os grupos disponíveis em uma organização, incluindo, entre outros, os grupos do Microsoft 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f752d667f854aa085530a97e68a90afa7fd26ba4
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373255"
---
# <a name="list-groups"></a><span data-ttu-id="b61fb-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="b61fb-103">List groups</span></span>

<span data-ttu-id="b61fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b61fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b61fb-105">Liste todos os grupos em uma organização, incluindo, entre outros, os grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b61fb-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="b61fb-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="b61fb-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="b61fb-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="b61fb-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="b61fb-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="b61fb-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="b61fb-109">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="b61fb-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="b61fb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b61fb-110">Permissions</span></span>

<span data-ttu-id="b61fb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b61fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b61fb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b61fb-113">Permission type</span></span> | <span data-ttu-id="b61fb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b61fb-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="b61fb-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b61fb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b61fb-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b61fb-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b61fb-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b61fb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b61fb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b61fb-118">Not supported.</span></span> |
| <span data-ttu-id="b61fb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b61fb-119">Application</span></span> | <span data-ttu-id="b61fb-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b61fb-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b61fb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b61fb-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b61fb-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b61fb-122">Optional query parameters</span></span>

<span data-ttu-id="b61fb-123">Para listar apenas grupos do Microsoft 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="b61fb-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="b61fb-124">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="b61fb-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="b61fb-125">Você também pode usar os `$count` e `$search` parâmetros de consulta para limitar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="b61fb-126">O `$search` parâmetro de consulta suporta a tokenização apenas nos campos **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="b61fb-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="b61fb-127">Outros campos são padrão para o `$filter` comportamento.</span><span class="sxs-lookup"><span data-stu-id="b61fb-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="b61fb-128">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b61fb-129">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="b61fb-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="b61fb-130">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b61fb-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b61fb-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-131">Request headers</span></span>

| <span data-ttu-id="b61fb-132">Nome</span><span class="sxs-lookup"><span data-stu-id="b61fb-132">Name</span></span> | <span data-ttu-id="b61fb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b61fb-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="b61fb-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="b61fb-134">Authorization</span></span>  | <span data-ttu-id="b61fb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b61fb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b61fb-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b61fb-137">ConsistencyLevel</span></span> | <span data-ttu-id="b61fb-138">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="b61fb-138">eventual.</span></span> <span data-ttu-id="b61fb-139">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="b61fb-140">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="b61fb-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b61fb-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-141">Request body</span></span>

<span data-ttu-id="b61fb-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b61fb-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b61fb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-143">Response</span></span>

<span data-ttu-id="b61fb-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="b61fb-145">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="b61fb-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="b61fb-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b61fb-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="b61fb-147">Exemplo 1: Obter uma lista de grupos</span><span class="sxs-lookup"><span data-stu-id="b61fb-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="b61fb-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-148">Request</span></span>

<span data-ttu-id="b61fb-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b61fb-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b61fb-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b61fb-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="b61fb-151">C#</span><span class="sxs-lookup"><span data-stu-id="b61fb-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b61fb-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b61fb-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b61fb-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b61fb-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b61fb-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-154">Response</span></span>

<span data-ttu-id="b61fb-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-155">The following is an example of the response.</span></span>
><span data-ttu-id="b61fb-156">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b61fb-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b61fb-157">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b61fb-157">All the default properties are returned for each group in an actual call.</span></span>

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

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="b61fb-158">Exemplo 2: Obter uma lista filtrada de grupos, incluindo a contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="b61fb-158">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b61fb-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b61fb-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="b61fb-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b61fb-161">C#</span><span class="sxs-lookup"><span data-stu-id="b61fb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b61fb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b61fb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b61fb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b61fb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b61fb-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-164">Response</span></span>

<span data-ttu-id="b61fb-165">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="b61fb-165">The following is an example of the response which includes only the requested properties.</span></span>

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

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="b61fb-166">Exemplo 3: Obter apenas uma contagem de grupos</span><span class="sxs-lookup"><span data-stu-id="b61fb-166">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="b61fb-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-167">Request</span></span>

<span data-ttu-id="b61fb-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b61fb-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b61fb-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="b61fb-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b61fb-170">C#</span><span class="sxs-lookup"><span data-stu-id="b61fb-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b61fb-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b61fb-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b61fb-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b61fb-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b61fb-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-173">Response</span></span>

<span data-ttu-id="b61fb-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="b61fb-175">893</span><span class="sxs-lookup"><span data-stu-id="b61fb-175">893</span></span>


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b61fb-176">Exemplo 4: Utilize $filter e $top para obter um grupo com um nome de exibição que comece com 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="b61fb-176">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b61fb-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-177">Request</span></span>

<span data-ttu-id="b61fb-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b61fb-178">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b61fb-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="b61fb-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b61fb-180">C#</span><span class="sxs-lookup"><span data-stu-id="b61fb-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b61fb-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b61fb-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b61fb-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b61fb-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b61fb-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-183">Response</span></span>

<span data-ttu-id="b61fb-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-184">The following is an example of the response.</span></span>
><span data-ttu-id="b61fb-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b61fb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="b61fb-187">Exemplo 5: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="b61fb-187">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b61fb-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-188">Request</span></span>

<span data-ttu-id="b61fb-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b61fb-189">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b61fb-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-190">Response</span></span>

<span data-ttu-id="b61fb-191">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-191">The following is an example of the response.</span></span>
><span data-ttu-id="b61fb-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b61fb-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="b61fb-194">Exemplo 6: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo' ou uma descrição que contenha as letras 'prod', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="b61fb-194">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b61fb-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b61fb-195">Request</span></span>

<span data-ttu-id="b61fb-196">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b61fb-196">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b61fb-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="b61fb-197">Response</span></span>

<span data-ttu-id="b61fb-198">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b61fb-198">The following is an example of the response.</span></span>
><span data-ttu-id="b61fb-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b61fb-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


