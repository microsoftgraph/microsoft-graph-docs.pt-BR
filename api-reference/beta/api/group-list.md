---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7024e456d672f1af49bd82c1b06c21ad57968f55
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236409"
---
# <a name="list-groups"></a><span data-ttu-id="361b5-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="361b5-103">List groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="361b5-104">Lista todos os grupos em uma organização, inclusive, mas não se limitando a, Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="361b5-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="361b5-105">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="361b5-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="361b5-106">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="361b5-106">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="361b5-107">Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="361b5-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="361b5-108">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="361b5-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="361b5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="361b5-109">Permissions</span></span>
<span data-ttu-id="361b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="361b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="361b5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="361b5-112">Permission type</span></span>      | <span data-ttu-id="361b5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="361b5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="361b5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="361b5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="361b5-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="361b5-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="361b5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="361b5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="361b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="361b5-117">Not supported.</span></span>    |
|<span data-ttu-id="361b5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="361b5-118">Application</span></span> | <span data-ttu-id="361b5-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="361b5-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="361b5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="361b5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="361b5-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="361b5-121">Optional query parameters</span></span>

<span data-ttu-id="361b5-122">Para listar apenas grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="361b5-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="361b5-123">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="361b5-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="361b5-124">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="361b5-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="361b5-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="361b5-125">Request headers</span></span>
| <span data-ttu-id="361b5-126">Nome</span><span class="sxs-lookup"><span data-stu-id="361b5-126">Name</span></span>       | <span data-ttu-id="361b5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="361b5-127">Type</span></span> | <span data-ttu-id="361b5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="361b5-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="361b5-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="361b5-129">Authorization</span></span>  | <span data-ttu-id="361b5-130">string</span><span class="sxs-lookup"><span data-stu-id="361b5-130">string</span></span>  | <span data-ttu-id="361b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="361b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="361b5-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="361b5-133">Request body</span></span>
<span data-ttu-id="361b5-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="361b5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="361b5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="361b5-135">Response</span></span>
<span data-ttu-id="361b5-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="361b5-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="361b5-137">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="361b5-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="361b5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="361b5-138">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="361b5-139">Exemplo 1: Retorna uma lista de objetos group.</span><span class="sxs-lookup"><span data-stu-id="361b5-139">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="361b5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="361b5-140">Request</span></span>

<span data-ttu-id="361b5-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="361b5-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response"></a><span data-ttu-id="361b5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="361b5-142">Response</span></span>

<span data-ttu-id="361b5-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="361b5-143">The following is an example of the response.</span></span>
><span data-ttu-id="361b5-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="361b5-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="361b5-145">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="361b5-145">All the default properties are returned for each group in an actual call.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="361b5-146">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="361b5-146">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="361b5-147">C#</span><span class="sxs-lookup"><span data-stu-id="361b5-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="361b5-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="361b5-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="361b5-149">Exemplo 2: Retorna uma lista filtrada de objetos group.</span><span class="sxs-lookup"><span data-stu-id="361b5-149">Example 2: Return a filtered list of group objects</span></span> 

#### <a name="request"></a><span data-ttu-id="361b5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="361b5-150">Request</span></span>

<span data-ttu-id="361b5-151">Este exemplo usa uma opção de consulta `$filter` para obter os grupos cujos membros tenham erros de licença, nas respectivas atribuições de licença baseadas em grupo.</span><span class="sxs-lookup"><span data-stu-id="361b5-151">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="361b5-152">Ele usa também uma opção de consulta `$select` para obter apenas as propriedades **id** e **displayName** de cada grupo na resposta, e não outras propriedades de retorno padrão ou não padrão.</span><span class="sxs-lookup"><span data-stu-id="361b5-152">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response"></a><span data-ttu-id="361b5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="361b5-153">Response</span></span>

<span data-ttu-id="361b5-154">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="361b5-154">The following is an example of the response which includes only the requested properties.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="361b5-155">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="361b5-155">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="361b5-156">C#</span><span class="sxs-lookup"><span data-stu-id="361b5-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="361b5-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="361b5-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
