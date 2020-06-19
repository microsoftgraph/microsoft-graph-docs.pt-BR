---
title: Obter primaryChannel
description: Recupere a propriedade de navegação de uma equipe que permite o acesso ao canal geral padrão.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c9be54f744e596b41de1d2e994dfe51b0c95e6d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791094"
---
# <a name="get-primarychannel"></a><span data-ttu-id="7ea02-103">Obter primaryChannel</span><span class="sxs-lookup"><span data-stu-id="7ea02-103">Get primaryChannel</span></span>

<span data-ttu-id="7ea02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ea02-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ea02-105">Recupere a propriedade de navegação de uma [equipe](../resources/team.md) que permite o acesso ao [canal](../resources/channel.md)geral padrão.</span><span class="sxs-lookup"><span data-stu-id="7ea02-105">Retrieve the navigation property of a [team](../resources/team.md) that allows access to the default General [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ea02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ea02-106">Permissions</span></span>
<span data-ttu-id="7ea02-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7ea02-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7ea02-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ea02-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ea02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ea02-109">Permission type</span></span>      | <span data-ttu-id="7ea02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ea02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ea02-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ea02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ea02-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ea02-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ea02-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ea02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ea02-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ea02-114">Not supported.</span></span>    |
|<span data-ttu-id="7ea02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ea02-115">Application</span></span> | <span data-ttu-id="7ea02-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ea02-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="7ea02-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="7ea02-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7ea02-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="7ea02-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7ea02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ea02-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel

```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ea02-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ea02-120">Optional query parameters</span></span>

<span data-ttu-id="7ea02-121">Este método oferece suporte a `$filter` , `$select` e a parâmetros de `$expand` [consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ea02-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ea02-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ea02-122">Request headers</span></span>
| <span data-ttu-id="7ea02-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ea02-123">Header</span></span>       | <span data-ttu-id="7ea02-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7ea02-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ea02-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ea02-125">Authorization</span></span>  | <span data-ttu-id="7ea02-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7ea02-126">Bearer {token}.</span></span> <span data-ttu-id="7ea02-127">Required.</span><span class="sxs-lookup"><span data-stu-id="7ea02-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ea02-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ea02-128">Request body</span></span>
<span data-ttu-id="7ea02-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ea02-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ea02-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ea02-130">Response</span></span>

<span data-ttu-id="7ea02-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ea02-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ea02-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ea02-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ea02-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ea02-133">Request</span></span>
<span data-ttu-id="7ea02-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ea02-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
### <a name="response"></a><span data-ttu-id="7ea02-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ea02-135">Response</span></span>
<span data-ttu-id="7ea02-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ea02-136">The following is an example of the response.</span></span> 

><span data-ttu-id="7ea02-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="7ea02-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ea02-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7ea02-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "isFavoriteByDefault": null,
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47",
    "membershipType": "standard"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get primaryChannel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
