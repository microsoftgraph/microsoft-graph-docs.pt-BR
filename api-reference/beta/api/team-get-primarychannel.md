---
title: Obter primaryChannel
description: Recupere a propriedade de navegação de uma equipe que permite o acesso ao canal geral padrão.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0993eb206abb4ddaea321567f4bc21a9ec22fbbe
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863443"
---
# <a name="get-primarychannel"></a><span data-ttu-id="aec1b-103">Obter primaryChannel</span><span class="sxs-lookup"><span data-stu-id="aec1b-103">Get primaryChannel</span></span>

<span data-ttu-id="aec1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec1b-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aec1b-105">Obter o [canal](../resources/channel.md)padrão, **geral**, de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="aec1b-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aec1b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aec1b-106">Permissions</span></span>
<span data-ttu-id="aec1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aec1b-109">Permission type</span></span>      | <span data-ttu-id="aec1b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aec1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aec1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aec1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aec1b-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec1b-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aec1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aec1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec1b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aec1b-114">Not supported.</span></span>    |
|<span data-ttu-id="aec1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aec1b-115">Application</span></span> | <span data-ttu-id="aec1b-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec1b-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="aec1b-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="aec1b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aec1b-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="aec1b-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aec1b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aec1b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aec1b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aec1b-120">Optional query parameters</span></span>

<span data-ttu-id="aec1b-121">Este método oferece suporte a `$filter` , `$select` e a parâmetros de `$expand` [consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aec1b-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aec1b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aec1b-122">Request headers</span></span>
| <span data-ttu-id="aec1b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aec1b-123">Header</span></span>       | <span data-ttu-id="aec1b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="aec1b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aec1b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aec1b-125">Authorization</span></span>  | <span data-ttu-id="aec1b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aec1b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aec1b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aec1b-128">Request body</span></span>
<span data-ttu-id="aec1b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aec1b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aec1b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec1b-130">Response</span></span>

<span data-ttu-id="aec1b-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aec1b-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aec1b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aec1b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="aec1b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec1b-133">Request</span></span>
<span data-ttu-id="aec1b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec1b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aec1b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aec1b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="aec1b-136">C#</span><span class="sxs-lookup"><span data-stu-id="aec1b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aec1b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aec1b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aec1b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aec1b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="aec1b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec1b-139">Response</span></span>
<span data-ttu-id="aec1b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aec1b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="aec1b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec1b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
