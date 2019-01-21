---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5081c5013c1bf7c1a1bfbcff58afe5a83aa67bc9
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726572"
---
# <a name="list-groups"></a><span data-ttu-id="6e3a9-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="6e3a9-103">List groups</span></span>
<span data-ttu-id="6e3a9-104">Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="6e3a9-105">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="6e3a9-106">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="6e3a9-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="6e3a9-107">Para obter propriedades _não_ retornadas por padrão, execute uma operação [GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="6e3a9-108">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="6e3a9-108">See an [example](group-get.md#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e3a9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e3a9-109">Permissions</span></span>
<span data-ttu-id="6e3a9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e3a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e3a9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e3a9-112">Permission type</span></span>      | <span data-ttu-id="6e3a9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e3a9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e3a9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e3a9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6e3a9-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e3a9-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e3a9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e3a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e3a9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-117">Not supported.</span></span>    |
|<span data-ttu-id="6e3a9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e3a9-118">Application</span></span> | <span data-ttu-id="6e3a9-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e3a9-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e3a9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e3a9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e3a9-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e3a9-121">Optional query parameters</span></span>
<span data-ttu-id="6e3a9-122">Para listar apenas Grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6e3a9-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="6e3a9-123">Use a opção de consulta `$orderby` do OData para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6e3a9-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="6e3a9-124">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6e3a9-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e3a9-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e3a9-125">Request headers</span></span>
| <span data-ttu-id="6e3a9-126">Nome</span><span class="sxs-lookup"><span data-stu-id="6e3a9-126">Name</span></span>       | <span data-ttu-id="6e3a9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e3a9-127">Type</span></span> | <span data-ttu-id="6e3a9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e3a9-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6e3a9-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e3a9-129">Authorization</span></span>  | <span data-ttu-id="6e3a9-130">string</span><span class="sxs-lookup"><span data-stu-id="6e3a9-130">string</span></span>  | <span data-ttu-id="6e3a9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e3a9-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e3a9-133">Request body</span></span>
<span data-ttu-id="6e3a9-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e3a9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e3a9-135">Response</span></span>
<span data-ttu-id="6e3a9-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="6e3a9-137">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="6e3a9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e3a9-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6e3a9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e3a9-139">Request</span></span>
<span data-ttu-id="6e3a9-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="6e3a9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e3a9-141">Response</span></span>
<span data-ttu-id="6e3a9-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-142">The following is an example of the response.</span></span>

><span data-ttu-id="6e3a9-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6e3a9-144">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e3a9-144">All the default properties are returned for each group in an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
