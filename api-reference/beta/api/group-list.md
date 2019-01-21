---
title: Listar grupos
description: Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 393381bfe5f21c4d4196251a4055fc65e0771e5c
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726600"
---
# <a name="list-groups"></a><span data-ttu-id="49ad6-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="49ad6-103">List groups</span></span>

> <span data-ttu-id="49ad6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="49ad6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49ad6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="49ad6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49ad6-106">Lista todos os grupos disponíveis em uma organização, inclusive, mas não limitado a Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="49ad6-106">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="49ad6-107">Esta operação retorna, por padrão, apenas um subconjunto das propriedades mais usadas de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="49ad6-107">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="49ad6-108">Essas propriedades _padrão_ estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="49ad6-108">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="49ad6-109">Para obter propriedades _não_ retornadas por padrão, execute uma operação [GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="49ad6-109">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="49ad6-110">Veja um [exemplo](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="49ad6-110">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="49ad6-111">A propriedade **hasMembersWithLicenseErrors** é uma exceção.</span><span class="sxs-lookup"><span data-stu-id="49ad6-111">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="49ad6-112">Veja um [exemplo](#request-2) de como usar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="49ad6-112">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="49ad6-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="49ad6-113">Permissions</span></span>
<span data-ttu-id="49ad6-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49ad6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49ad6-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49ad6-116">Permission type</span></span>      | <span data-ttu-id="49ad6-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49ad6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49ad6-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49ad6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="49ad6-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ad6-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49ad6-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49ad6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49ad6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49ad6-121">Not supported.</span></span>    |
|<span data-ttu-id="49ad6-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49ad6-122">Application</span></span> | <span data-ttu-id="49ad6-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ad6-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49ad6-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49ad6-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49ad6-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49ad6-125">Optional query parameters</span></span>

<span data-ttu-id="49ad6-126">Para listar apenas Grupos do Office 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49ad6-126">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="49ad6-127">Use a opção de consulta `$orderby` do OData para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49ad6-127">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="49ad6-128">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49ad6-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49ad6-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49ad6-129">Request headers</span></span>
| <span data-ttu-id="49ad6-130">Nome</span><span class="sxs-lookup"><span data-stu-id="49ad6-130">Name</span></span>       | <span data-ttu-id="49ad6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="49ad6-131">Type</span></span> | <span data-ttu-id="49ad6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="49ad6-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="49ad6-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="49ad6-133">Authorization</span></span>  | <span data-ttu-id="49ad6-134">string</span><span class="sxs-lookup"><span data-stu-id="49ad6-134">string</span></span>  | <span data-ttu-id="49ad6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49ad6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49ad6-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49ad6-137">Request body</span></span>
<span data-ttu-id="49ad6-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49ad6-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49ad6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ad6-139">Response</span></span>
<span data-ttu-id="49ad6-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49ad6-140">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="49ad6-141">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="49ad6-141">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="49ad6-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49ad6-142">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="49ad6-143">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="49ad6-143">Request 1</span></span>
<span data-ttu-id="49ad6-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49ad6-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response-1"></a><span data-ttu-id="49ad6-145">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="49ad6-145">Response 1</span></span>
<span data-ttu-id="49ad6-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49ad6-146">The following is an example of the response.</span></span>
><span data-ttu-id="49ad6-147">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="49ad6-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49ad6-148">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49ad6-148">All the default properties are returned for each group in an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="49ad6-149">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="49ad6-149">Request 2</span></span>
<span data-ttu-id="49ad6-150">Este exemplo usa uma opção de consulta `$filter` para obter os grupos cujos membros tenham erros de licença, nas respectivas atribuições de licença baseadas em grupo.</span><span class="sxs-lookup"><span data-stu-id="49ad6-150">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="49ad6-151">Ele usa também uma opção de consulta `$select` para obter apenas as propriedades **id** e **displayName** de cada grupo na resposta, e não outras propriedades de retorno padrão ou não padrão.</span><span class="sxs-lookup"><span data-stu-id="49ad6-151">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="49ad6-152">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="49ad6-152">Response 2</span></span>
<span data-ttu-id="49ad6-153">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="49ad6-153">The following is an example of the response which includes only the requested properties.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
