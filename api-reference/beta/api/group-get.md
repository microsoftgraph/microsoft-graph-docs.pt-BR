---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 99215af564be186edaf57563ae493f363c9cc2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941048"
---
# <a name="get-group"></a><span data-ttu-id="d67b8-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="d67b8-103">Get group</span></span>

> <span data-ttu-id="d67b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d67b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d67b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d67b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d67b8-106">Obtenha as propriedades e relacionamentos de um objeto [group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="d67b8-106">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="d67b8-107">Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="d67b8-107">Default properties</span></span>

<span data-ttu-id="d67b8-p102">O seguinte item representa o conjunto padrão de propriedades que são retornadas ao obter ou listar grupos. Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d67b8-p102">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="d67b8-110">classificação</span><span class="sxs-lookup"><span data-stu-id="d67b8-110">classification</span></span>
* <span data-ttu-id="d67b8-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d67b8-111">createdDateTime</span></span>
* <span data-ttu-id="d67b8-112">description</span><span class="sxs-lookup"><span data-stu-id="d67b8-112">description</span></span>
* <span data-ttu-id="d67b8-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d67b8-113">displayName</span></span>
* <span data-ttu-id="d67b8-114">groupTypes</span><span class="sxs-lookup"><span data-stu-id="d67b8-114">groupTypes</span></span>
* <span data-ttu-id="d67b8-115">id</span><span class="sxs-lookup"><span data-stu-id="d67b8-115">id</span></span>
* <span data-ttu-id="d67b8-116">Email</span><span class="sxs-lookup"><span data-stu-id="d67b8-116">mail</span></span>
* <span data-ttu-id="d67b8-117">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="d67b8-117">mailEnabled</span></span>
* <span data-ttu-id="d67b8-118">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d67b8-118">mailNickname</span></span>
* <span data-ttu-id="d67b8-119">membershipRule</span><span class="sxs-lookup"><span data-stu-id="d67b8-119">membershipRule</span></span>
* <span data-ttu-id="d67b8-120">membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="d67b8-120">membershipRuleProcessingState</span></span>
* <span data-ttu-id="d67b8-121">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d67b8-121">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="d67b8-122">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d67b8-122">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="d67b8-123">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="d67b8-123">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="d67b8-124">preferredLanguage - não suportado; um valor para essa propriedade não pode ser definida e retorna `null` quando chamado.</span><span class="sxs-lookup"><span data-stu-id="d67b8-124">preferredLanguage - Not supported; a value for this property cannot be set and returns `null` when called.</span></span>
* <span data-ttu-id="d67b8-125">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="d67b8-125">proxyAddresses</span></span>
* <span data-ttu-id="d67b8-126">renewedDateTime</span><span class="sxs-lookup"><span data-stu-id="d67b8-126">renewedDateTime</span></span>
* <span data-ttu-id="d67b8-127">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="d67b8-127">securityEnabled</span></span>
* <span data-ttu-id="d67b8-128">tema</span><span class="sxs-lookup"><span data-stu-id="d67b8-128">theme</span></span>
* <span data-ttu-id="d67b8-129">visibilidade</span><span class="sxs-lookup"><span data-stu-id="d67b8-129">visibility</span></span>

<span data-ttu-id="d67b8-130">As seguintes propriedades de grupo não são retornadas por padrão:</span><span class="sxs-lookup"><span data-stu-id="d67b8-130">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="d67b8-131">accessType</span><span class="sxs-lookup"><span data-stu-id="d67b8-131">accessType</span></span>
* <span data-ttu-id="d67b8-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="d67b8-132">allowExternalSenders</span></span>
* <span data-ttu-id="d67b8-133">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="d67b8-133">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="d67b8-134">hasMembersWithLicenseErrors</span><span class="sxs-lookup"><span data-stu-id="d67b8-134">hasMembersWithLicenseErrors</span></span>
* <span data-ttu-id="d67b8-135">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="d67b8-135">isSubscribedByMail</span></span>
* <span data-ttu-id="d67b8-136">isFavorite</span><span class="sxs-lookup"><span data-stu-id="d67b8-136">isFavorite</span></span>
* <span data-ttu-id="d67b8-137">unseenConversationsCount</span><span class="sxs-lookup"><span data-stu-id="d67b8-137">unseenConversationsCount</span></span>
* <span data-ttu-id="d67b8-138">unseenCount</span><span class="sxs-lookup"><span data-stu-id="d67b8-138">unseenCount</span></span>
* <span data-ttu-id="d67b8-139">unseenMessagesCount</span><span class="sxs-lookup"><span data-stu-id="d67b8-139">unseenMessagesCount</span></span>

<span data-ttu-id="d67b8-140">Para fazer essas propriedades (exceto **isFavorite** e **hasMembersWithLicenseErrors**), use o `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="d67b8-140">To get these properties (except **isFavorite** and **hasMembersWithLicenseErrors**), use the `$select` query parameter.</span></span> <span data-ttu-id="d67b8-141">Eis alguns exemplos:</span><span class="sxs-lookup"><span data-stu-id="d67b8-141">The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

<span data-ttu-id="d67b8-142">Para retornar os grupos que contêm membros com erros de licença, use o parâmetro de consulta **$filter** :</span><span class="sxs-lookup"><span data-stu-id="d67b8-142">To return groups containing members with license errors, use the **$filter** query parameter:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

<span data-ttu-id="d67b8-143">Desde que o recurso de **grupo** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância de **grupo** .</span><span class="sxs-lookup"><span data-stu-id="d67b8-143">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="d67b8-144">Permissions</span><span class="sxs-lookup"><span data-stu-id="d67b8-144">Permissions</span></span>
<span data-ttu-id="d67b8-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d67b8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d67b8-147">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d67b8-147">Permission type</span></span>      | <span data-ttu-id="d67b8-148">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d67b8-148">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d67b8-149">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d67b8-149">Delegated (work or school account)</span></span> | <span data-ttu-id="d67b8-150">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d67b8-150">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d67b8-151">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d67b8-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d67b8-152">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d67b8-152">Not supported.</span></span>    |
|<span data-ttu-id="d67b8-153">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d67b8-153">Application</span></span> | <span data-ttu-id="d67b8-154">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d67b8-154">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d67b8-155">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d67b8-155">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d67b8-156">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d67b8-156">Optional query parameters</span></span>
<span data-ttu-id="d67b8-157">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d67b8-157">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d67b8-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d67b8-158">Request headers</span></span>
| <span data-ttu-id="d67b8-159">Nome</span><span class="sxs-lookup"><span data-stu-id="d67b8-159">Name</span></span>       | <span data-ttu-id="d67b8-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="d67b8-160">Type</span></span> | <span data-ttu-id="d67b8-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="d67b8-161">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d67b8-162">Autorização</span><span class="sxs-lookup"><span data-stu-id="d67b8-162">Authorization</span></span>  | <span data-ttu-id="d67b8-163">string</span><span class="sxs-lookup"><span data-stu-id="d67b8-163">string</span></span>  | <span data-ttu-id="d67b8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d67b8-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d67b8-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d67b8-166">Request body</span></span>
<span data-ttu-id="d67b8-167">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d67b8-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d67b8-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d67b8-168">Response</span></span>
<span data-ttu-id="d67b8-169">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d67b8-169">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d67b8-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d67b8-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="d67b8-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d67b8-171">Request</span></span>
<span data-ttu-id="d67b8-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d67b8-172">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="d67b8-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="d67b8-173">Response</span></span>
<span data-ttu-id="d67b8-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d67b8-174">The following is an example of the response.</span></span> 
><span data-ttu-id="d67b8-175">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d67b8-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d67b8-176">As propriedades padrão serão retornadas de uma chamada real, conforme descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="d67b8-176">The default properties will be returned from an actual call, as described before.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d67b8-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="d67b8-177">See also</span></span>

- [<span data-ttu-id="d67b8-178">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d67b8-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d67b8-179">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="d67b8-179">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d67b8-180">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="d67b8-180">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
