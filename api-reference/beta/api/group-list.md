---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4e0069df916b3a29759ee164c15aac7dc1fcb2ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419098"
---
# <a name="list-groups"></a><span data-ttu-id="7636e-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="7636e-103">List groups</span></span>

<span data-ttu-id="7636e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7636e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7636e-105">Lista todos os grupos em uma organização, inclusive, mas não se limitando a, Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7636e-105">List all the groups in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="7636e-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="7636e-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="7636e-107">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="7636e-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="7636e-108">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="7636e-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="7636e-109">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="7636e-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="7636e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7636e-110">Permissions</span></span>
<span data-ttu-id="7636e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7636e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7636e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7636e-113">Permission type</span></span>      | <span data-ttu-id="7636e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7636e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7636e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7636e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7636e-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7636e-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7636e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7636e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7636e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7636e-118">Not supported.</span></span>    |
|<span data-ttu-id="7636e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7636e-119">Application</span></span> | <span data-ttu-id="7636e-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7636e-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7636e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7636e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7636e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7636e-122">Optional query parameters</span></span>

<span data-ttu-id="7636e-123">Para listar apenas grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="7636e-123">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="7636e-124">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="7636e-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="7636e-125">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7636e-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7636e-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7636e-126">Request headers</span></span>
| <span data-ttu-id="7636e-127">Nome</span><span class="sxs-lookup"><span data-stu-id="7636e-127">Name</span></span>       | <span data-ttu-id="7636e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7636e-128">Type</span></span> | <span data-ttu-id="7636e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7636e-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7636e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7636e-130">Authorization</span></span>  | <span data-ttu-id="7636e-131">string</span><span class="sxs-lookup"><span data-stu-id="7636e-131">string</span></span>  | <span data-ttu-id="7636e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7636e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7636e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7636e-134">Request body</span></span>
<span data-ttu-id="7636e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7636e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7636e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7636e-136">Response</span></span>
<span data-ttu-id="7636e-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7636e-137">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="7636e-138">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="7636e-138">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="7636e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7636e-139">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="7636e-140">Exemplo 1: Retorna uma lista de objetos group</span><span class="sxs-lookup"><span data-stu-id="7636e-140">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="7636e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7636e-141">Request</span></span>

<span data-ttu-id="7636e-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7636e-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7636e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7636e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="7636e-144">C#</span><span class="sxs-lookup"><span data-stu-id="7636e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7636e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7636e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7636e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7636e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7636e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7636e-147">Response</span></span>

<span data-ttu-id="7636e-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7636e-148">The following is an example of the response.</span></span>
><span data-ttu-id="7636e-149">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7636e-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7636e-150">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7636e-150">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
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


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="7636e-151">Exemplo 2: Retorna uma lista filtrada de objetos de grupo</span><span class="sxs-lookup"><span data-stu-id="7636e-151">Example 2: Return a filtered list of group objects</span></span> 

#### <a name="request"></a><span data-ttu-id="7636e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7636e-152">Request</span></span>

<span data-ttu-id="7636e-153">Este exemplo usa uma opção de consulta `$filter` para obter os grupos cujos membros tenham erros de licença, nas respectivas atribuições de licença baseadas em grupo.</span><span class="sxs-lookup"><span data-stu-id="7636e-153">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="7636e-154">Ele usa também uma opção de consulta `$select` para obter apenas as propriedades **id** e **displayName** de cada grupo na resposta, e não outras propriedades de retorno padrão ou não padrão.</span><span class="sxs-lookup"><span data-stu-id="7636e-154">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="7636e-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7636e-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="c"></a>[<span data-ttu-id="7636e-156">C#</span><span class="sxs-lookup"><span data-stu-id="7636e-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7636e-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7636e-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7636e-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7636e-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7636e-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7636e-159">Response</span></span>

<span data-ttu-id="7636e-160">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="7636e-160">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups_withlicenseerrors"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
    "value": [
        {
            "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
            "displayName": "Library Assist"
        },
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "displayName": "Golf Assist"
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
