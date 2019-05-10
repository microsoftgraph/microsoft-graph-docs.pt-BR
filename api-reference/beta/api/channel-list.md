---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 476f5a698801725ce441c31d21715a2a180658cf
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635502"
---
# <a name="list-channels"></a><span data-ttu-id="6db40-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="6db40-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6db40-104">Recuperar a lista de [canais](../resources/channel.md) nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="6db40-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6db40-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6db40-105">Permissions</span></span>
<span data-ttu-id="6db40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6db40-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6db40-108">Permission type</span></span>      | <span data-ttu-id="6db40-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6db40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6db40-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6db40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6db40-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db40-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6db40-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6db40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db40-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db40-113">Not supported.</span></span>    |
|<span data-ttu-id="6db40-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6db40-114">Application</span></span> | <span data-ttu-id="6db40-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db40-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="6db40-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6db40-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6db40-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="6db40-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6db40-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6db40-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6db40-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6db40-119">Optional query parameters</span></span>
<span data-ttu-id="6db40-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6db40-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6db40-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6db40-121">Request headers</span></span>
| <span data-ttu-id="6db40-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6db40-122">Header</span></span>       | <span data-ttu-id="6db40-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6db40-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6db40-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6db40-124">Authorization</span></span>  | <span data-ttu-id="6db40-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6db40-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6db40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6db40-127">Request body</span></span>
<span data-ttu-id="6db40-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6db40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6db40-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db40-129">Response</span></span>

<span data-ttu-id="6db40-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6db40-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db40-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6db40-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6db40-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db40-132">Request</span></span>
<span data-ttu-id="6db40-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db40-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="6db40-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db40-134">Response</span></span>
<span data-ttu-id="6db40-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6db40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6db40-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6db40-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6db40-139">C#</span><span class="sxs-lookup"><span data-stu-id="6db40-139">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channels-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6db40-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="6db40-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channels-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
