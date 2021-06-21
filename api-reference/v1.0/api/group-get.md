---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 63860da9bcb2c87c30577ce34f067f315efe15e9
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030933"
---
# <a name="get-group"></a><span data-ttu-id="88504-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="88504-103">Get group</span></span>

<span data-ttu-id="88504-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88504-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88504-105">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="88504-105">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="88504-106">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="88504-106">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="88504-107">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="88504-107">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="88504-108">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="88504-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="88504-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="88504-109">Permissions</span></span>
<span data-ttu-id="88504-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88504-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88504-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88504-112">Permission type</span></span>      | <span data-ttu-id="88504-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88504-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88504-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88504-114">Delegated (work or school account)</span></span> | <span data-ttu-id="88504-115">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="88504-115">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="88504-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88504-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88504-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88504-117">Not supported.</span></span>    |
|<span data-ttu-id="88504-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88504-118">Application</span></span> | <span data-ttu-id="88504-119">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="88504-119">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="88504-120">**Observação:** dependendo dos recursos de grupo que você está tentando acessar, as permissões podem ser limitadas.</span><span class="sxs-lookup"><span data-stu-id="88504-120">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="88504-121">Para obter mais informações, consulte a seção [Grupos](/graph/known-issues#groups) em [Problemas conhecidos com o Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="88504-121">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="88504-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88504-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88504-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88504-123">Optional query parameters</span></span>
<span data-ttu-id="88504-124">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="88504-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="88504-125">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="88504-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="88504-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88504-126">Request headers</span></span>
| <span data-ttu-id="88504-127">Nome</span><span class="sxs-lookup"><span data-stu-id="88504-127">Name</span></span>       | <span data-ttu-id="88504-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="88504-128">Type</span></span> | <span data-ttu-id="88504-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="88504-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="88504-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="88504-130">Authorization</span></span>  | <span data-ttu-id="88504-131">string</span><span class="sxs-lookup"><span data-stu-id="88504-131">string</span></span>  | <span data-ttu-id="88504-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88504-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88504-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88504-134">Request body</span></span>
<span data-ttu-id="88504-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88504-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88504-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="88504-136">Response</span></span>
<span data-ttu-id="88504-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88504-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="88504-138">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="88504-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="88504-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88504-139">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="88504-140">Exemplo 1: Retornar todas as propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="88504-140">Example 1: Return all default properties</span></span>

<span data-ttu-id="88504-141">Retornar todas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="88504-141">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="88504-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88504-142">Request</span></span> 

<span data-ttu-id="88504-143">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="88504-143">The following is an example of a GET request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="88504-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="88504-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```
# <a name="c"></a>[<span data-ttu-id="88504-145">C#</span><span class="sxs-lookup"><span data-stu-id="88504-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88504-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88504-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88504-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88504-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88504-148">Java</span><span class="sxs-lookup"><span data-stu-id="88504-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="88504-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="88504-149">Response</span></span>
<span data-ttu-id="88504-p106">Veja a seguir o exemplo de uma resposta. Ela inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="88504-p106">The following is an example of the response. It includes only the default properties.</span></span>

><span data-ttu-id="88504-p107">**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura. Todas as propriedades padrão são retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88504-p107">**Note:** The response object shown here might be shortened for readability. All the default properties are returned in an actual call.</span></span>

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
    "isAssignableToRole": null,
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


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="88504-154">Exemplo 2: Retornar propriedades adicionais usando $select</span><span class="sxs-lookup"><span data-stu-id="88504-154">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="88504-155">Retornar propriedades adicionais usando `$select`.</span><span class="sxs-lookup"><span data-stu-id="88504-155">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="88504-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88504-156">Request</span></span>

<span data-ttu-id="88504-157">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="88504-157">The following is an example of a GET request.</span></span>


# <a name="http"></a>[<span data-ttu-id="88504-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="88504-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="c"></a>[<span data-ttu-id="88504-159">C#</span><span class="sxs-lookup"><span data-stu-id="88504-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88504-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88504-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88504-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88504-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88504-162">Java</span><span class="sxs-lookup"><span data-stu-id="88504-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="88504-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="88504-163">Response</span></span>

<span data-ttu-id="88504-164">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="88504-164">The following is an example of the response which includes the requested non-default properties.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

