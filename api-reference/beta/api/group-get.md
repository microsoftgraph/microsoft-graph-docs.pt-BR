---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 9ac99ad0e31a355ea81c47a313d3440c985753a1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593152"
---
# <a name="get-group"></a><span data-ttu-id="01b0f-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="01b0f-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01b0f-104">Obtenha as propriedades e os relacionamentos de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="01b0f-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

<span data-ttu-id="01b0f-105">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="01b0f-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="01b0f-106">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="01b0f-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="01b0f-107">Veja um [exemplo](#request-2) de `$select`.</span><span class="sxs-lookup"><span data-stu-id="01b0f-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="01b0f-108">A propriedade **hasMembersWithLicenseErrors** é uma exceção.</span><span class="sxs-lookup"><span data-stu-id="01b0f-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="01b0f-109">Veja um [exemplo](group-list.md#request-2) de como usar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="01b0f-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="01b0f-110">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **group**.</span><span class="sxs-lookup"><span data-stu-id="01b0f-110">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="01b0f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="01b0f-111">Permissions</span></span>
<span data-ttu-id="01b0f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01b0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01b0f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01b0f-114">Permission type</span></span>      | <span data-ttu-id="01b0f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01b0f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01b0f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01b0f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="01b0f-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01b0f-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01b0f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01b0f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01b0f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01b0f-119">Not supported.</span></span>    |
|<span data-ttu-id="01b0f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01b0f-120">Application</span></span> | <span data-ttu-id="01b0f-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01b0f-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01b0f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01b0f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01b0f-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01b0f-123">Optional query parameters</span></span>
<span data-ttu-id="01b0f-124">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="01b0f-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="01b0f-125">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="01b0f-125">See an [example](#request-2) below.</span></span>

<span data-ttu-id="01b0f-126">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="01b0f-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="01b0f-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01b0f-127">Request headers</span></span>
| <span data-ttu-id="01b0f-128">Nome</span><span class="sxs-lookup"><span data-stu-id="01b0f-128">Name</span></span>       | <span data-ttu-id="01b0f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="01b0f-129">Type</span></span> | <span data-ttu-id="01b0f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="01b0f-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01b0f-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="01b0f-131">Authorization</span></span>  | <span data-ttu-id="01b0f-132">string</span><span class="sxs-lookup"><span data-stu-id="01b0f-132">string</span></span>  | <span data-ttu-id="01b0f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01b0f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01b0f-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01b0f-135">Request body</span></span>
<span data-ttu-id="01b0f-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01b0f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01b0f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="01b0f-137">Response</span></span>
<span data-ttu-id="01b0f-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01b0f-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="01b0f-139">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="01b0f-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="01b0f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01b0f-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="01b0f-141">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="01b0f-141">Request 1</span></span>
<span data-ttu-id="01b0f-142">Este é um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="01b0f-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="01b0f-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="01b0f-143">Response 1</span></span>
<span data-ttu-id="01b0f-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01b0f-144">The following is an example of the response.</span></span> <span data-ttu-id="01b0f-145">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="01b0f-145">It includes only the default properties.</span></span>

><span data-ttu-id="01b0f-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="01b0f-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="01b0f-147">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01b0f-147">All the default properties are returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="01b0f-148">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="01b0f-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="01b0f-149">C#</span><span class="sxs-lookup"><span data-stu-id="01b0f-149">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01b0f-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="01b0f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="01b0f-151">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="01b0f-151">Request 2</span></span>
<span data-ttu-id="01b0f-152">O exemplo a seguir usa uma opção de consulta `$select` para obter algumas propriedades não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="01b0f-152">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="01b0f-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="01b0f-153">Response 2</span></span>
<span data-ttu-id="01b0f-154">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="01b0f-154">The following is an example of the response which includes the requested non-default properties.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="01b0f-155">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="01b0f-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="01b0f-156">C#</span><span class="sxs-lookup"><span data-stu-id="01b0f-156">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01b0f-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="01b0f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="01b0f-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="01b0f-158">See also</span></span>

- [<span data-ttu-id="01b0f-159">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="01b0f-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="01b0f-160">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="01b0f-160">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="01b0f-161">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="01b0f-161">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
