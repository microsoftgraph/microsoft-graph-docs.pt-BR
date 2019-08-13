---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2723c18d964cd29a11da54ddd2356dc28824ab8d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317432"
---
# <a name="list-channels"></a><span data-ttu-id="4e14f-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="4e14f-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e14f-104">Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4e14f-104">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e14f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e14f-105">Permissions</span></span>
<span data-ttu-id="4e14f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e14f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e14f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e14f-108">Permission type</span></span>      | <span data-ttu-id="4e14f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e14f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e14f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e14f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e14f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e14f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e14f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e14f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e14f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e14f-113">Not supported.</span></span>    |
|<span data-ttu-id="4e14f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e14f-114">Application</span></span> | <span data-ttu-id="4e14f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e14f-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="4e14f-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4e14f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4e14f-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="4e14f-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e14f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e14f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e14f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4e14f-119">Optional query parameters</span></span>
<span data-ttu-id="4e14f-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4e14f-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e14f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e14f-121">Request headers</span></span>
| <span data-ttu-id="4e14f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e14f-122">Header</span></span>       | <span data-ttu-id="4e14f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4e14f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e14f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e14f-124">Authorization</span></span>  | <span data-ttu-id="4e14f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e14f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e14f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e14f-127">Request body</span></span>
<span data-ttu-id="4e14f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e14f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e14f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e14f-129">Response</span></span>

<span data-ttu-id="4e14f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e14f-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e14f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e14f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e14f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e14f-132">Request</span></span>
<span data-ttu-id="4e14f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e14f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e14f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e14f-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e14f-135">C#</span><span class="sxs-lookup"><span data-stu-id="4e14f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e14f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e14f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e14f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e14f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4e14f-138">Java</span><span class="sxs-lookup"><span data-stu-id="4e14f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e14f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e14f-139">Response</span></span>
<span data-ttu-id="4e14f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e14f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
