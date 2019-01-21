---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 321e24ef8b36547a4823578d7f6823397d0eed69
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726593"
---
# <a name="get-group"></a><span data-ttu-id="66c04-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="66c04-103">Get group</span></span>
<span data-ttu-id="66c04-104">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="66c04-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="66c04-105">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="66c04-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="66c04-106">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="66c04-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="66c04-107">Veja um [exemplo](#request-2).</span><span class="sxs-lookup"><span data-stu-id="66c04-107">See an [example](#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="66c04-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="66c04-108">Permissions</span></span>
<span data-ttu-id="66c04-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66c04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66c04-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66c04-111">Permission type</span></span>      | <span data-ttu-id="66c04-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66c04-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66c04-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66c04-113">Delegated (work or school account)</span></span> | <span data-ttu-id="66c04-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66c04-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="66c04-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66c04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66c04-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66c04-116">Not supported.</span></span>    |
|<span data-ttu-id="66c04-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66c04-117">Application</span></span> | <span data-ttu-id="66c04-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66c04-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66c04-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66c04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66c04-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66c04-120">Optional query parameters</span></span>
<span data-ttu-id="66c04-121">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="66c04-121">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="66c04-122">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="66c04-122">See an [example](#request-2).</span></span>

<span data-ttu-id="66c04-123">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="66c04-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="66c04-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66c04-124">Request headers</span></span>
| <span data-ttu-id="66c04-125">Nome</span><span class="sxs-lookup"><span data-stu-id="66c04-125">Name</span></span>       | <span data-ttu-id="66c04-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="66c04-126">Type</span></span> | <span data-ttu-id="66c04-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="66c04-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66c04-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="66c04-128">Authorization</span></span>  | <span data-ttu-id="66c04-129">string</span><span class="sxs-lookup"><span data-stu-id="66c04-129">string</span></span>  | <span data-ttu-id="66c04-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66c04-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66c04-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66c04-132">Request body</span></span>
<span data-ttu-id="66c04-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66c04-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66c04-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="66c04-134">Response</span></span>
<span data-ttu-id="66c04-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66c04-135">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66c04-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66c04-136">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="66c04-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="66c04-137">Request 1</span></span>
<span data-ttu-id="66c04-138">Este é um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="66c04-138">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="66c04-139">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="66c04-139">Response 1</span></span>
<span data-ttu-id="66c04-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66c04-140">The following is an example of the response.</span></span> <span data-ttu-id="66c04-141">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="66c04-141">It includes only the default properties.</span></span>

><span data-ttu-id="66c04-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66c04-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="66c04-143">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66c04-143">All the default properties are returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-22T00:51:37Z",
    "creationOptions": [],
    "description": "Self help community for library",
    "displayName": "Library Assist",
    "groupTypes": [
        "Unified"
    ],
    "mail": "library2@contoso.com",
    "mailEnabled": true,
    "mailNickname": "library",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "smtp:library7423@contoso.com",
        "SMTP:library2@contoso.com"
    ],
    "renewedDateTime": "2018-12-22T00:51:37Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="66c04-144">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="66c04-144">Request 2</span></span>
<span data-ttu-id="66c04-145">O exemplo a seguir usa uma opção de consulta `$select` para obter algumas propriedades não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="66c04-145">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="66c04-146">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="66c04-146">Response 2</span></span>
<span data-ttu-id="66c04-147">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="66c04-147">The following is an example of the response which includes the requested non-default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
