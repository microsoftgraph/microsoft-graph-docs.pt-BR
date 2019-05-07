---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: aad378eaa82b5550f4d021b283c8437187fdf8c1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613807"
---
# <a name="list-groups"></a><span data-ttu-id="e8d69-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="e8d69-103">List groups</span></span>
<span data-ttu-id="e8d69-104">Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e8d69-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="e8d69-105">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="e8d69-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e8d69-106">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="e8d69-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="e8d69-107">Para obter propriedades _não_ retornadas por padrão, execute uma operação [GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="e8d69-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="e8d69-108">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="e8d69-108">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="e8d69-109">A propriedade **hasMembersWithLicenseErrors** é uma exceção.</span><span class="sxs-lookup"><span data-stu-id="e8d69-109">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="e8d69-110">Veja um [exemplo](#request-2) de como usar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="e8d69-110">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d69-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8d69-111">Permissions</span></span>
<span data-ttu-id="e8d69-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d69-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d69-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8d69-114">Permission type</span></span>      | <span data-ttu-id="e8d69-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8d69-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d69-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8d69-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e8d69-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8d69-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8d69-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8d69-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d69-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8d69-119">Not supported.</span></span>    |
|<span data-ttu-id="e8d69-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8d69-120">Application</span></span> | <span data-ttu-id="e8d69-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8d69-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8d69-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d69-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8d69-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8d69-123">Optional query parameters</span></span>
<span data-ttu-id="e8d69-124">Para listar apenas grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="e8d69-124">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="e8d69-125">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="e8d69-125">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="e8d69-126">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8d69-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8d69-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d69-127">Request headers</span></span>
| <span data-ttu-id="e8d69-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e8d69-128">Name</span></span>       | <span data-ttu-id="e8d69-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8d69-129">Type</span></span> | <span data-ttu-id="e8d69-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d69-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8d69-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8d69-131">Authorization</span></span>  | <span data-ttu-id="e8d69-132">string</span><span class="sxs-lookup"><span data-stu-id="e8d69-132">string</span></span>  | <span data-ttu-id="e8d69-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8d69-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8d69-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d69-135">Request body</span></span>
<span data-ttu-id="e8d69-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8d69-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8d69-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d69-137">Response</span></span>
<span data-ttu-id="e8d69-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d69-138">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="e8d69-139">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="e8d69-139">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="e8d69-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8d69-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e8d69-141">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e8d69-141">Request 1</span></span>
<span data-ttu-id="e8d69-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8d69-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response-1"></a><span data-ttu-id="e8d69-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e8d69-143">Response 1</span></span>
<span data-ttu-id="e8d69-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d69-144">The following is an example of the response.</span></span>

><span data-ttu-id="e8d69-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8d69-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8d69-146">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8d69-146">All the default properties are returned for each group in an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "creationOptions": [],
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "creationOptions": [],
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8d69-147">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e8d69-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8d69-148">C#</span><span class="sxs-lookup"><span data-stu-id="e8d69-148">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8d69-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8d69-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
#### <a name="request-2"></a><span data-ttu-id="e8d69-150">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e8d69-150">Request 2</span></span>
<span data-ttu-id="e8d69-151">Este exemplo usa uma opção de consulta `$filter` para obter os grupos cujos membros tenham erros de licença, nas respectivas atribuições de licença baseadas em grupo.</span><span class="sxs-lookup"><span data-stu-id="e8d69-151">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="e8d69-152">Ele usa também uma opção de consulta `$select` para obter apenas as propriedades **id** e **displayName** de cada grupo na resposta, e não outras propriedades de retorno padrão ou não padrão.</span><span class="sxs-lookup"><span data-stu-id="e8d69-152">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="e8d69-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e8d69-153">Response 2</span></span>
<span data-ttu-id="e8d69-154">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="e8d69-154">The following is an example of the response which includes only the requested properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8d69-155">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e8d69-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8d69-156">C#</span><span class="sxs-lookup"><span data-stu-id="e8d69-156">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8d69-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8d69-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
