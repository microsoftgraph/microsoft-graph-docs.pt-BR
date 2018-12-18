---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
ms.openlocfilehash: dc61d3d42f95b47649183f2dbc0932b4b4327400
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358027"
---
# <a name="get-group"></a><span data-ttu-id="11562-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="11562-103">Get group</span></span>

> <span data-ttu-id="11562-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11562-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11562-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11562-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11562-106">Obtenha as propriedades e relacionamentos de um objeto [group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="11562-106">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="11562-107">Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="11562-107">Default properties</span></span>

<span data-ttu-id="11562-p102">O seguinte item representa o conjunto padrão de propriedades que são retornadas ao obter ou listar grupos. Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="11562-p102">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="11562-110">classificação</span><span class="sxs-lookup"><span data-stu-id="11562-110">classification</span></span>
* <span data-ttu-id="11562-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11562-111">createdDateTime</span></span>
* <span data-ttu-id="11562-112">description</span><span class="sxs-lookup"><span data-stu-id="11562-112">description</span></span>
* <span data-ttu-id="11562-113">displayName</span><span class="sxs-lookup"><span data-stu-id="11562-113">displayName</span></span>
* <span data-ttu-id="11562-114">groupTypes</span><span class="sxs-lookup"><span data-stu-id="11562-114">groupTypes</span></span>
* <span data-ttu-id="11562-115">id</span><span class="sxs-lookup"><span data-stu-id="11562-115">id</span></span>
* <span data-ttu-id="11562-116">Email</span><span class="sxs-lookup"><span data-stu-id="11562-116">mail</span></span>
* <span data-ttu-id="11562-117">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="11562-117">mailEnabled</span></span>
* <span data-ttu-id="11562-118">mailNickname</span><span class="sxs-lookup"><span data-stu-id="11562-118">mailNickname</span></span>
* <span data-ttu-id="11562-119">membershipRule</span><span class="sxs-lookup"><span data-stu-id="11562-119">membershipRule</span></span>
* <span data-ttu-id="11562-120">membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="11562-120">membershipRuleProcessingState</span></span>
* <span data-ttu-id="11562-121">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="11562-121">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="11562-122">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="11562-122">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="11562-123">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="11562-123">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="11562-124">preferredLanguage - não suportado; um valor para essa propriedade não pode ser definida e retorna `null` quando chamado.</span><span class="sxs-lookup"><span data-stu-id="11562-124">preferredLanguage - Not supported; a value for this property cannot be set and returns `null` when called.</span></span>
* <span data-ttu-id="11562-125">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="11562-125">proxyAddresses</span></span>
* <span data-ttu-id="11562-126">renewedDateTime</span><span class="sxs-lookup"><span data-stu-id="11562-126">renewedDateTime</span></span>
* <span data-ttu-id="11562-127">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="11562-127">securityEnabled</span></span>
* <span data-ttu-id="11562-128">tema</span><span class="sxs-lookup"><span data-stu-id="11562-128">theme</span></span>
* <span data-ttu-id="11562-129">visibilidade</span><span class="sxs-lookup"><span data-stu-id="11562-129">visibility</span></span>

<span data-ttu-id="11562-130">As seguintes propriedades de grupo não são retornadas por padrão:</span><span class="sxs-lookup"><span data-stu-id="11562-130">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="11562-131">accessType</span><span class="sxs-lookup"><span data-stu-id="11562-131">accessType</span></span>
* <span data-ttu-id="11562-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="11562-132">allowExternalSenders</span></span>
* <span data-ttu-id="11562-133">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="11562-133">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="11562-134">hasMembersWithLicenseErrors</span><span class="sxs-lookup"><span data-stu-id="11562-134">hasMembersWithLicenseErrors</span></span>
* <span data-ttu-id="11562-135">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="11562-135">isSubscribedByMail</span></span>
* <span data-ttu-id="11562-136">isFavorite</span><span class="sxs-lookup"><span data-stu-id="11562-136">isFavorite</span></span>
* <span data-ttu-id="11562-137">unseenConversationsCount</span><span class="sxs-lookup"><span data-stu-id="11562-137">unseenConversationsCount</span></span>
* <span data-ttu-id="11562-138">unseenCount</span><span class="sxs-lookup"><span data-stu-id="11562-138">unseenCount</span></span>
* <span data-ttu-id="11562-139">unseenMessagesCount</span><span class="sxs-lookup"><span data-stu-id="11562-139">unseenMessagesCount</span></span>

<span data-ttu-id="11562-140">Para fazer essas propriedades (exceto **isFavorite** e **hasMembersWithLicenseErrors**), use o `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="11562-140">To get these properties (except **isFavorite** and **hasMembersWithLicenseErrors**), use the `$select` query parameter.</span></span> <span data-ttu-id="11562-141">Eis alguns exemplos:</span><span class="sxs-lookup"><span data-stu-id="11562-141">The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

<span data-ttu-id="11562-142">Para retornar os grupos que contêm membros com erros de licença, use o parâmetro de consulta **$filter** :</span><span class="sxs-lookup"><span data-stu-id="11562-142">To return groups containing members with license errors, use the **$filter** query parameter:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

<span data-ttu-id="11562-143">Desde que o recurso de **grupo** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância de **grupo** .</span><span class="sxs-lookup"><span data-stu-id="11562-143">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="11562-144">Permissões</span><span class="sxs-lookup"><span data-stu-id="11562-144">Permissions</span></span>
<span data-ttu-id="11562-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11562-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11562-147">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11562-147">Permission type</span></span>      | <span data-ttu-id="11562-148">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11562-148">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11562-149">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11562-149">Delegated (work or school account)</span></span> | <span data-ttu-id="11562-150">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11562-150">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="11562-151">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11562-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11562-152">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11562-152">Not supported.</span></span>    |
|<span data-ttu-id="11562-153">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11562-153">Application</span></span> | <span data-ttu-id="11562-154">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11562-154">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11562-155">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11562-155">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="11562-156">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11562-156">Optional query parameters</span></span>
<span data-ttu-id="11562-157">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="11562-157">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11562-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11562-158">Request headers</span></span>
| <span data-ttu-id="11562-159">Nome</span><span class="sxs-lookup"><span data-stu-id="11562-159">Name</span></span>       | <span data-ttu-id="11562-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="11562-160">Type</span></span> | <span data-ttu-id="11562-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="11562-161">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11562-162">Autorização</span><span class="sxs-lookup"><span data-stu-id="11562-162">Authorization</span></span>  | <span data-ttu-id="11562-163">string</span><span class="sxs-lookup"><span data-stu-id="11562-163">string</span></span>  | <span data-ttu-id="11562-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11562-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11562-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11562-166">Request body</span></span>
<span data-ttu-id="11562-167">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11562-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11562-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="11562-168">Response</span></span>
<span data-ttu-id="11562-169">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11562-169">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11562-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11562-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="11562-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11562-171">Request</span></span>
<span data-ttu-id="11562-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11562-172">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="11562-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="11562-173">Response</span></span>
<span data-ttu-id="11562-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11562-174">The following is an example of the response.</span></span> 
><span data-ttu-id="11562-175">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11562-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="11562-176">As propriedades padrão serão retornadas de uma chamada real, conforme descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="11562-176">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

## <a name="see-also"></a><span data-ttu-id="11562-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="11562-177">See also</span></span>

- [<span data-ttu-id="11562-178">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="11562-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="11562-179">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="11562-179">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="11562-180">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="11562-180">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
