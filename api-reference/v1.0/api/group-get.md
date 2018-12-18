---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: dkershaw10
ms.openlocfilehash: aed805172759971740d1576b4b3040934116cd66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340310"
---
# <a name="get-group"></a><span data-ttu-id="fe1fd-103">Obter grupo</span><span class="sxs-lookup"><span data-stu-id="fe1fd-103">Get group</span></span>
<span data-ttu-id="fe1fd-104">Obtenha as propriedades e os relacionamentos de um objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="fe1fd-105">Propriedades padrão</span><span class="sxs-lookup"><span data-stu-id="fe1fd-105">Default properties</span></span>

<span data-ttu-id="fe1fd-p101">O seguinte item representa o conjunto padrão de propriedades que são retornadas ao obter ou listar grupos. Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="fe1fd-108">description</span><span class="sxs-lookup"><span data-stu-id="fe1fd-108">description</span></span>
* <span data-ttu-id="fe1fd-109">displayName</span><span class="sxs-lookup"><span data-stu-id="fe1fd-109">displayName</span></span>
* <span data-ttu-id="fe1fd-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="fe1fd-110">groupTypes</span></span>
* <span data-ttu-id="fe1fd-111">id</span><span class="sxs-lookup"><span data-stu-id="fe1fd-111">id</span></span>
* <span data-ttu-id="fe1fd-112">Email</span><span class="sxs-lookup"><span data-stu-id="fe1fd-112">mail</span></span>
* <span data-ttu-id="fe1fd-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="fe1fd-113">mailEnabled</span></span>
* <span data-ttu-id="fe1fd-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fe1fd-114">mailNickname</span></span>
* <span data-ttu-id="fe1fd-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fe1fd-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="fe1fd-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe1fd-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="fe1fd-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="fe1fd-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="fe1fd-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="fe1fd-118">proxyAddresses</span></span>
* <span data-ttu-id="fe1fd-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="fe1fd-119">securityEnabled</span></span>
* <span data-ttu-id="fe1fd-120">visibilidade</span><span class="sxs-lookup"><span data-stu-id="fe1fd-120">visibility</span></span>

<span data-ttu-id="fe1fd-121">As seguintes propriedades de grupo não são retornadas por padrão:</span><span class="sxs-lookup"><span data-stu-id="fe1fd-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="fe1fd-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="fe1fd-122">allowExternalSenders</span></span>
* <span data-ttu-id="fe1fd-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="fe1fd-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="fe1fd-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="fe1fd-124">isSubscribedByMail</span></span>
* <span data-ttu-id="fe1fd-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="fe1fd-125">unseenCount</span></span>

<span data-ttu-id="fe1fd-p102">Para obter essas propriedades, use o parâmetro de consulta **$select**. Eis alguns exemplos:</span><span class="sxs-lookup"><span data-stu-id="fe1fd-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="fe1fd-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe1fd-128">Permissions</span></span>
<span data-ttu-id="fe1fd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe1fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe1fd-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe1fd-131">Permission type</span></span>      | <span data-ttu-id="fe1fd-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe1fd-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe1fd-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe1fd-133">Delegated (work or school account)</span></span> | <span data-ttu-id="fe1fd-134">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe1fd-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe1fd-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe1fd-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe1fd-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-136">Not supported.</span></span>    |
|<span data-ttu-id="fe1fd-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe1fd-137">Application</span></span> | <span data-ttu-id="fe1fd-138">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe1fd-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe1fd-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe1fd-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe1fd-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe1fd-140">Optional query parameters</span></span>
<span data-ttu-id="fe1fd-141">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe1fd-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1fd-142">Request headers</span></span>
| <span data-ttu-id="fe1fd-143">Nome</span><span class="sxs-lookup"><span data-stu-id="fe1fd-143">Name</span></span>       | <span data-ttu-id="fe1fd-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe1fd-144">Type</span></span> | <span data-ttu-id="fe1fd-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe1fd-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe1fd-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe1fd-146">Authorization</span></span>  | <span data-ttu-id="fe1fd-147">string</span><span class="sxs-lookup"><span data-stu-id="fe1fd-147">string</span></span>  | <span data-ttu-id="fe1fd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe1fd-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1fd-150">Request body</span></span>
<span data-ttu-id="fe1fd-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe1fd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe1fd-152">Response</span></span>
<span data-ttu-id="fe1fd-153">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe1fd-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe1fd-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fe1fd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1fd-155">Request</span></span>
<span data-ttu-id="fe1fd-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="fe1fd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe1fd-157">Response</span></span>
<span data-ttu-id="fe1fd-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-158">The following is an example of the response.</span></span>

><span data-ttu-id="fe1fd-159">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe1fd-160">As propriedades padrão serão retornadas de uma chamada real, conforme descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="fe1fd-160">The default properties will be returned from an actual call, as described before.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
