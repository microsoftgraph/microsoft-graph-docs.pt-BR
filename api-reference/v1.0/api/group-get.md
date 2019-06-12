---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 4eb677622f56e6bd575a6c391b9ddc08bea4fc2f
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812765"
---
# <a name="get-group"></a><span data-ttu-id="e3ae1-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="e3ae1-103">Get group</span></span>
<span data-ttu-id="e3ae1-104">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="e3ae1-105">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="e3ae1-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="e3ae1-106">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="e3ae1-107">Veja um [exemplo](#request-2) de `$select`.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="e3ae1-108">A propriedade **hasMembersWithLicenseErrors** é uma exceção.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="e3ae1-109">Veja um [exemplo](group-list.md#request-2) de como usar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ae1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3ae1-110">Permissions</span></span>
<span data-ttu-id="e3ae1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ae1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ae1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3ae1-113">Permission type</span></span>      | <span data-ttu-id="e3ae1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3ae1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3ae1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3ae1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e3ae1-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3ae1-116">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e3ae1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3ae1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ae1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-118">Not supported.</span></span>    |
|<span data-ttu-id="e3ae1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3ae1-119">Application</span></span> | <span data-ttu-id="e3ae1-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3ae1-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3ae1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ae1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3ae1-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3ae1-122">Optional query parameters</span></span>
<span data-ttu-id="e3ae1-123">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="e3ae1-124">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-124">See an [example](#request-2) below.</span></span>

<span data-ttu-id="e3ae1-125">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e3ae1-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3ae1-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ae1-126">Request headers</span></span>
| <span data-ttu-id="e3ae1-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e3ae1-127">Name</span></span>       | <span data-ttu-id="e3ae1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3ae1-128">Type</span></span> | <span data-ttu-id="e3ae1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3ae1-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3ae1-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3ae1-130">Authorization</span></span>  | <span data-ttu-id="e3ae1-131">string</span><span class="sxs-lookup"><span data-stu-id="e3ae1-131">string</span></span>  | <span data-ttu-id="e3ae1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3ae1-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ae1-134">Request body</span></span>
<span data-ttu-id="e3ae1-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3ae1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ae1-136">Response</span></span>
<span data-ttu-id="e3ae1-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e3ae1-138">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="e3ae1-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3ae1-139">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e3ae1-140">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e3ae1-140">Request 1</span></span>
<span data-ttu-id="e3ae1-141">Este é um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-141">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="e3ae1-142">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e3ae1-142">Response 1</span></span>
<span data-ttu-id="e3ae1-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-143">The following is an example of the response.</span></span> <span data-ttu-id="e3ae1-144">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-144">It includes only the default properties.</span></span>

><span data-ttu-id="e3ae1-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e3ae1-146">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-146">All the default properties are returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3ae1-147">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e3ae1-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3ae1-148">C#</span><span class="sxs-lookup"><span data-stu-id="e3ae1-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3ae1-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3ae1-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="e3ae1-150">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e3ae1-150">Request 2</span></span>
<span data-ttu-id="e3ae1-151">O exemplo a seguir usa uma opção de consulta `$select` para obter algumas propriedades não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-151">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="e3ae1-152">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e3ae1-152">Response 2</span></span>
<span data-ttu-id="e3ae1-153">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e3ae1-153">The following is an example of the response which includes the requested non-default properties.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3ae1-154">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e3ae1-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3ae1-155">C#</span><span class="sxs-lookup"><span data-stu-id="e3ae1-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3ae1-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3ae1-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
