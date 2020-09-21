---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8496383023781f796389bfbaf616bc0c64b9e97e
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843251"
---
# <a name="list-channels"></a><span data-ttu-id="72cc1-103">Listar canais</span><span class="sxs-lookup"><span data-stu-id="72cc1-103">List channels</span></span>

<span data-ttu-id="72cc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72cc1-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="72cc1-105">Recuperar a lista de [canais](../resources/channel.md) nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="72cc1-105">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="72cc1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72cc1-106">Permissions</span></span>
<span data-ttu-id="72cc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72cc1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72cc1-109">Permission type</span></span>      | <span data-ttu-id="72cc1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72cc1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72cc1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72cc1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72cc1-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cc1-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="72cc1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72cc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72cc1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72cc1-114">Not supported.</span></span>    |
|<span data-ttu-id="72cc1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72cc1-115">Application</span></span> | <span data-ttu-id="72cc1-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cc1-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="72cc1-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="72cc1-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="72cc1-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="72cc1-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="72cc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72cc1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72cc1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72cc1-120">Optional query parameters</span></span>
<span data-ttu-id="72cc1-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72cc1-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72cc1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72cc1-122">Request headers</span></span>
| <span data-ttu-id="72cc1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72cc1-123">Header</span></span>       | <span data-ttu-id="72cc1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="72cc1-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72cc1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72cc1-125">Authorization</span></span>  | <span data-ttu-id="72cc1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72cc1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72cc1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72cc1-128">Request body</span></span>
<span data-ttu-id="72cc1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72cc1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72cc1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="72cc1-130">Response</span></span>

<span data-ttu-id="72cc1-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72cc1-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72cc1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72cc1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72cc1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72cc1-133">Request</span></span>
<span data-ttu-id="72cc1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72cc1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72cc1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="72cc1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="72cc1-136">C#</span><span class="sxs-lookup"><span data-stu-id="72cc1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72cc1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72cc1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72cc1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72cc1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72cc1-139">Java</span><span class="sxs-lookup"><span data-stu-id="72cc1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72cc1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="72cc1-140">Response</span></span>
<span data-ttu-id="72cc1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72cc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
