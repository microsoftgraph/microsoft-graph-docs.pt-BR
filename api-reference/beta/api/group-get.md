---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 84cdad08c3c227487c603bbfb5268d71aac85332
ms.sourcegitcommit: 6714f71e0d229f1ab56150a9976b5106b4c8b785
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2020
ms.locfileid: "49368170"
---
# <a name="get-group"></a><span data-ttu-id="c78b0-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="c78b0-103">Get group</span></span>

<span data-ttu-id="c78b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c78b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c78b0-105">Obtenha as propriedades e os relacionamentos de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="c78b0-105">Get the properties and relationships of a [group](../resources/group.md) object.</span></span> 

<span data-ttu-id="c78b0-106">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="c78b0-106">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="c78b0-107">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="c78b0-107">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="c78b0-108">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="c78b0-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span> <span data-ttu-id="c78b0-109">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **group**.</span><span class="sxs-lookup"><span data-stu-id="c78b0-109">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="c78b0-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c78b0-110">Permissions</span></span>
<span data-ttu-id="c78b0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c78b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c78b0-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c78b0-113">Permission type</span></span>      | <span data-ttu-id="c78b0-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c78b0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c78b0-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c78b0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c78b0-116">GroupMember. Read. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c78b0-116">GroupMember.Read.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="c78b0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c78b0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c78b0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c78b0-118">Not supported.</span></span>    |
|<span data-ttu-id="c78b0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c78b0-119">Application</span></span> | <span data-ttu-id="c78b0-120">GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c78b0-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="c78b0-121">**Observação:** dependendo dos recursos de grupo que você está tentando acessar, as permissões podem ser limitadas.</span><span class="sxs-lookup"><span data-stu-id="c78b0-121">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="c78b0-122">Para obter mais informações, consulte a seção [Grupos](/graph/known-issues#groups) em [Problemas conhecidos com o Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="c78b0-122">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="c78b0-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c78b0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c78b0-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c78b0-124">Optional query parameters</span></span>
<span data-ttu-id="c78b0-125">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="c78b0-125">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="c78b0-126">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c78b0-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c78b0-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c78b0-127">Request headers</span></span>
| <span data-ttu-id="c78b0-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c78b0-128">Name</span></span>       | <span data-ttu-id="c78b0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c78b0-129">Type</span></span> | <span data-ttu-id="c78b0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c78b0-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c78b0-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c78b0-131">Authorization</span></span>  | <span data-ttu-id="c78b0-132">string</span><span class="sxs-lookup"><span data-stu-id="c78b0-132">string</span></span>  | <span data-ttu-id="c78b0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c78b0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c78b0-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c78b0-135">Request body</span></span>
<span data-ttu-id="c78b0-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c78b0-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c78b0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c78b0-137">Response</span></span>
<span data-ttu-id="c78b0-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c78b0-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="c78b0-139">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="c78b0-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="c78b0-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c78b0-140">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="c78b0-141">Exemplo 1: Retornar todas as propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="c78b0-141">Example 1: Return all default properties</span></span>

#### <a name="request"></a><span data-ttu-id="c78b0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c78b0-142">Request</span></span>

<span data-ttu-id="c78b0-143">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="c78b0-143">The following is an example of a GET request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="c78b0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c78b0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```
# <a name="c"></a>[<span data-ttu-id="c78b0-145">C#</span><span class="sxs-lookup"><span data-stu-id="c78b0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c78b0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c78b0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c78b0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c78b0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c78b0-148">Java</span><span class="sxs-lookup"><span data-stu-id="c78b0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c78b0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c78b0-149">Response</span></span>
<span data-ttu-id="c78b0-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c78b0-150">The following is an example of the response.</span></span> <span data-ttu-id="c78b0-151">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="c78b0-151">It includes only the default properties.</span></span>

><span data-ttu-id="c78b0-152">**Observação:** O objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c78b0-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c78b0-153">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c78b0-153">All the default properties are returned in an actual call.</span></span>
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
  "isAssignableToRole": null,
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


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="c78b0-154">Exemplo 2: Retornar propriedades adicionais usando $select</span><span class="sxs-lookup"><span data-stu-id="c78b0-154">Example 2: Return additional properties by using $select</span></span>

#### <a name="request"></a><span data-ttu-id="c78b0-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c78b0-155">Request</span></span>

<span data-ttu-id="c78b0-156">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="c78b0-156">The following is an example of a GET request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c78b0-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c78b0-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="c"></a>[<span data-ttu-id="c78b0-158">C#</span><span class="sxs-lookup"><span data-stu-id="c78b0-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c78b0-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c78b0-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c78b0-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c78b0-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c78b0-161">Java</span><span class="sxs-lookup"><span data-stu-id="c78b0-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c78b0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c78b0-162">Response</span></span>

<span data-ttu-id="c78b0-163">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="c78b0-163">The following is an example of the response which includes the requested non-default properties.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="c78b0-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="c78b0-164">See also</span></span>

- [<span data-ttu-id="c78b0-165">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c78b0-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c78b0-166">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="c78b0-166">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c78b0-167">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="c78b0-167">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->


