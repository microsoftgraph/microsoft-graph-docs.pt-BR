---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: b00d6a076de377b9cf0c393c443aa619b3d7ab48
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324100"
---
# <a name="get-group"></a><span data-ttu-id="96565-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="96565-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96565-104">Obtenha as propriedades e os relacionamentos de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="96565-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

<span data-ttu-id="96565-105">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="96565-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="96565-106">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="96565-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="96565-107">Veja um [exemplo](#request-2) de `$select`.</span><span class="sxs-lookup"><span data-stu-id="96565-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="96565-108">A propriedade **hasMembersWithLicenseErrors** é uma exceção.</span><span class="sxs-lookup"><span data-stu-id="96565-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="96565-109">Veja um [exemplo](group-list.md#request-2) de como usar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="96565-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="96565-110">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **group**.</span><span class="sxs-lookup"><span data-stu-id="96565-110">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="96565-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="96565-111">Permissions</span></span>
<span data-ttu-id="96565-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96565-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96565-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96565-114">Permission type</span></span>      | <span data-ttu-id="96565-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96565-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96565-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96565-116">Delegated (work or school account)</span></span> | <span data-ttu-id="96565-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96565-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96565-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96565-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96565-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96565-119">Not supported.</span></span>    |
|<span data-ttu-id="96565-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96565-120">Application</span></span> | <span data-ttu-id="96565-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96565-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96565-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96565-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96565-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96565-123">Optional query parameters</span></span>
<span data-ttu-id="96565-124">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="96565-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="96565-125">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="96565-125">See an [example](#request-2) below.</span></span>

<span data-ttu-id="96565-126">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="96565-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="96565-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96565-127">Request headers</span></span>
| <span data-ttu-id="96565-128">Nome</span><span class="sxs-lookup"><span data-stu-id="96565-128">Name</span></span>       | <span data-ttu-id="96565-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="96565-129">Type</span></span> | <span data-ttu-id="96565-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="96565-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96565-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="96565-131">Authorization</span></span>  | <span data-ttu-id="96565-132">string</span><span class="sxs-lookup"><span data-stu-id="96565-132">string</span></span>  | <span data-ttu-id="96565-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96565-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96565-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96565-135">Request body</span></span>
<span data-ttu-id="96565-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96565-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96565-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="96565-137">Response</span></span>
<span data-ttu-id="96565-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96565-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="96565-139">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="96565-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="96565-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96565-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="96565-141">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="96565-141">Request 1</span></span>
<span data-ttu-id="96565-142">Este é um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="96565-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="96565-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="96565-143">Response 1</span></span>
<span data-ttu-id="96565-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96565-144">The following is an example of the response.</span></span> <span data-ttu-id="96565-145">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="96565-145">It includes only the default properties.</span></span>

><span data-ttu-id="96565-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="96565-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="96565-147">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96565-147">All the default properties are returned in an actual call.</span></span>
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
}
```

#### <a name="request-2"></a><span data-ttu-id="96565-148">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="96565-148">Request 2</span></span>
<span data-ttu-id="96565-149">O exemplo a seguir usa uma opção de consulta `$select` para obter algumas propriedades não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="96565-149">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="96565-150">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="96565-150">Response 2</span></span>
<span data-ttu-id="96565-151">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="96565-151">The following is an example of the response which includes the requested non-default properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

## <a name="see-also"></a><span data-ttu-id="96565-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="96565-152">See also</span></span>

- [<span data-ttu-id="96565-153">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="96565-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="96565-154">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="96565-154">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="96565-155">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="96565-155">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
