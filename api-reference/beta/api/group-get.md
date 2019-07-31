---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 43482bfa8e8024a134ee12d7e50f0a33df373596
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953882"
---
# <a name="get-group"></a><span data-ttu-id="1b892-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="1b892-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b892-104">Obtenha as propriedades e os relacionamentos de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="1b892-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span> 

<span data-ttu-id="1b892-105">Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="1b892-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="1b892-106">Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="1b892-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="1b892-107">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="1b892-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span> <span data-ttu-id="1b892-108">Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **group**.</span><span class="sxs-lookup"><span data-stu-id="1b892-108">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b892-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b892-109">Permissions</span></span>
<span data-ttu-id="1b892-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b892-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b892-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b892-112">Permission type</span></span>      | <span data-ttu-id="1b892-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b892-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b892-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b892-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1b892-115">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b892-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="1b892-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b892-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b892-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b892-117">Not supported.</span></span>    |
|<span data-ttu-id="1b892-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b892-118">Application</span></span> | <span data-ttu-id="1b892-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b892-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="1b892-120">**Observação:** dependendo dos recursos de grupo que você está tentando acessar, as permissões podem ser limitadas.</span><span class="sxs-lookup"><span data-stu-id="1b892-120">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="1b892-121">Para obter mais informações, consulte a seção [Grupos](/graph/known-issues#groups) em [Problemas conhecidos com o Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="1b892-121">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="1b892-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b892-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b892-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b892-123">Optional query parameters</span></span>
<span data-ttu-id="1b892-124">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="1b892-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="1b892-125">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b892-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b892-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b892-126">Request headers</span></span>
| <span data-ttu-id="1b892-127">Nome</span><span class="sxs-lookup"><span data-stu-id="1b892-127">Name</span></span>       | <span data-ttu-id="1b892-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b892-128">Type</span></span> | <span data-ttu-id="1b892-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b892-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1b892-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b892-130">Authorization</span></span>  | <span data-ttu-id="1b892-131">string</span><span class="sxs-lookup"><span data-stu-id="1b892-131">string</span></span>  | <span data-ttu-id="1b892-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b892-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b892-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b892-134">Request body</span></span>
<span data-ttu-id="1b892-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b892-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b892-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b892-136">Response</span></span>
<span data-ttu-id="1b892-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b892-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="1b892-138">Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="1b892-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="1b892-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b892-139">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="1b892-140">Exemplo 1: Retornar todas as propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="1b892-140">Example 1: Return all default properties</span></span>

#### <a name="request"></a><span data-ttu-id="1b892-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b892-141">Request</span></span>

<span data-ttu-id="1b892-142">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="1b892-142">The following is an example of a GET request.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="1b892-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b892-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b892-144">C#</span><span class="sxs-lookup"><span data-stu-id="1b892-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b892-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b892-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b892-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b892-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b892-147">Java</span><span class="sxs-lookup"><span data-stu-id="1b892-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b892-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b892-148">Response</span></span>
<span data-ttu-id="1b892-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b892-149">The following is an example of the response.</span></span> <span data-ttu-id="1b892-150">Ele inclui apenas as propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="1b892-150">It includes only the default properties.</span></span>

><span data-ttu-id="1b892-151">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b892-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1b892-152">Todas as propriedades padrão serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b892-152">All the default properties are returned in an actual call.</span></span>
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


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="1b892-153">Exemplo 2: Retornar propriedades adicionais usando $select</span><span class="sxs-lookup"><span data-stu-id="1b892-153">Example 2: Return additional properties by using $select</span></span>

#### <a name="request"></a><span data-ttu-id="1b892-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b892-154">Request</span></span>

<span data-ttu-id="1b892-155">Veja a seguir um exemplo de solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="1b892-155">The following is an example of a GET request.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="1b892-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b892-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b892-157">C#</span><span class="sxs-lookup"><span data-stu-id="1b892-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b892-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b892-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b892-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b892-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b892-160">Java</span><span class="sxs-lookup"><span data-stu-id="1b892-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b892-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b892-161">Response</span></span>

<span data-ttu-id="1b892-162">Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="1b892-162">The following is an example of the response which includes the requested non-default properties.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="1b892-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="1b892-163">See also</span></span>

- [<span data-ttu-id="1b892-164">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1b892-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1b892-165">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="1b892-165">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1b892-166">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="1b892-166">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
