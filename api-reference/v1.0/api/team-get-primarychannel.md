---
title: Get primaryChannel
description: Recupere a propriedade de navegação de uma equipe que permita acesso ao seu canal Geral padrão.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 50f3bc5fd03c509afe73616bc79ba3cd1582bfe6
ms.sourcegitcommit: 95c1cf4f70a9322d276dc84726457eeaf98169e2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2020
ms.locfileid: "46531506"
---
# <a name="get-primarychannel"></a><span data-ttu-id="086ba-103">Get primaryChannel</span><span class="sxs-lookup"><span data-stu-id="086ba-103">Get primaryChannel</span></span>

<span data-ttu-id="086ba-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="086ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="086ba-105">Obtenha o canal [padrão](../resources/channel.md), **Geral**, de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="086ba-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="086ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="086ba-106">Permissions</span></span>
<span data-ttu-id="086ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="086ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="086ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="086ba-109">Permission type</span></span>      | <span data-ttu-id="086ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="086ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="086ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="086ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="086ba-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="086ba-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="086ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="086ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="086ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="086ba-114">Not supported.</span></span>    |
|<span data-ttu-id="086ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="086ba-115">Application</span></span> | <span data-ttu-id="086ba-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="086ba-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="086ba-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="086ba-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="086ba-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="086ba-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="086ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="086ba-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="086ba-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="086ba-120">Optional query parameters</span></span>

<span data-ttu-id="086ba-121">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="086ba-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="086ba-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="086ba-122">Request headers</span></span>
| <span data-ttu-id="086ba-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="086ba-123">Header</span></span>       | <span data-ttu-id="086ba-124">Valor</span><span class="sxs-lookup"><span data-stu-id="086ba-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="086ba-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="086ba-125">Authorization</span></span>  | <span data-ttu-id="086ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="086ba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="086ba-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="086ba-128">Request body</span></span>
<span data-ttu-id="086ba-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="086ba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="086ba-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="086ba-130">Response</span></span>

<span data-ttu-id="086ba-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="086ba-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="086ba-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="086ba-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="086ba-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="086ba-133">Request</span></span>
<span data-ttu-id="086ba-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="086ba-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="086ba-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="086ba-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="086ba-136">C#</span><span class="sxs-lookup"><span data-stu-id="086ba-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="086ba-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="086ba-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="086ba-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="086ba-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="086ba-139">Java</span><span class="sxs-lookup"><span data-stu-id="086ba-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-primarychannel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="086ba-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="086ba-140">Response</span></span>
<span data-ttu-id="086ba-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="086ba-141">The following is an example of the response.</span></span> 

><span data-ttu-id="086ba-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="086ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47"
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
