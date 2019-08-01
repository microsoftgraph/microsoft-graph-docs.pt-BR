---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dd12ee9f078545b6ad486056e37335c28c70935c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014939"
---
# <a name="get-group"></a><span data-ttu-id="e085f-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="e085f-103">Get group</span></span>

<span data-ttu-id="e085f-104">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="e085f-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="e085f-105">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="e085f-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="e085f-106">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="e085f-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="e085f-107">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="e085f-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="e085f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e085f-108">Permissions</span></span>
<span data-ttu-id="e085f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e085f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e085f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e085f-111">Permission type</span></span>      | <span data-ttu-id="e085f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e085f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e085f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e085f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e085f-114">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e085f-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e085f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e085f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e085f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e085f-116">Not supported.</span></span>    |
|<span data-ttu-id="e085f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e085f-117">Application</span></span> | <span data-ttu-id="e085f-118">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e085f-118">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="e085f-119">**Observação:** dependendo dos recursos de grupo que você está tentando acessar, as permissões podem ser limitadas.</span><span class="sxs-lookup"><span data-stu-id="e085f-119">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="e085f-120">Para obter mais informações, consulte a seção [Grupos](/graph/known-issues#groups) em [Problemas conhecidos com o Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="e085f-120">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="e085f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e085f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e085f-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e085f-122">Optional query parameters</span></span>
<span data-ttu-id="e085f-123">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e085f-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="e085f-124">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e085f-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e085f-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e085f-125">Request headers</span></span>
| <span data-ttu-id="e085f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="e085f-126">Name</span></span>       | <span data-ttu-id="e085f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e085f-127">Type</span></span> | <span data-ttu-id="e085f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e085f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e085f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e085f-129">Authorization</span></span>  | <span data-ttu-id="e085f-130">string</span><span class="sxs-lookup"><span data-stu-id="e085f-130">string</span></span>  | <span data-ttu-id="e085f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e085f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e085f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e085f-133">Request body</span></span>
<span data-ttu-id="e085f-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e085f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e085f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e085f-135">Response</span></span>
<span data-ttu-id="e085f-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e085f-136">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e085f-137">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="e085f-137">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="e085f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e085f-138">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="e085f-139">Exemplo 1: Retornar todas as propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="e085f-139">Example 1: Return all default properties</span></span>

<span data-ttu-id="e085f-140">Retornar todas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="e085f-140">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="e085f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e085f-141">Request</span></span> 

<span data-ttu-id="e085f-142">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="e085f-142">The following is an example of a GET request.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="e085f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e085f-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e085f-144">C#</span><span class="sxs-lookup"><span data-stu-id="e085f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e085f-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="e085f-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e085f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e085f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e085f-147">Java</span><span class="sxs-lookup"><span data-stu-id="e085f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e085f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e085f-148">Response</span></span>
<span data-ttu-id="e085f-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e085f-149">The following is an example of the response.</span></span> <span data-ttu-id="e085f-150">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="e085f-150">It includes only the default properties.</span></span>

><span data-ttu-id="e085f-151">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e085f-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e085f-152">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e085f-152">All the default properties are returned in an actual call.</span></span>

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


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="e085f-153">Exemplo 2: Retornar propriedades adicionais usando $select</span><span class="sxs-lookup"><span data-stu-id="e085f-153">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="e085f-154">Retornar propriedades adicionais usando `$select`.</span><span class="sxs-lookup"><span data-stu-id="e085f-154">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="e085f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e085f-155">Request</span></span>

<span data-ttu-id="e085f-156">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="e085f-156">The following is an example of a GET request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e085f-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e085f-157">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e085f-158">C#</span><span class="sxs-lookup"><span data-stu-id="e085f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e085f-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="e085f-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e085f-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e085f-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e085f-161">Java</span><span class="sxs-lookup"><span data-stu-id="e085f-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e085f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e085f-162">Response</span></span>

<span data-ttu-id="e085f-163">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e085f-163">The following is an example of the response which includes the requested non-default properties.</span></span>

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
