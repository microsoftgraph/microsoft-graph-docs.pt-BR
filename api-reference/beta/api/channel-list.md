---
title: Canais de lista
description: Recupere a lista de canais nesse conjunto.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6900b0a64721556b5020baee197e4c7f78d90278
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936162"
---
# <a name="list-channels"></a><span data-ttu-id="d855c-103">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="d855c-103">List channels</span></span>

> <span data-ttu-id="d855c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d855c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d855c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d855c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d855c-106">Recupere a lista de [canais](../resources/channel.md) nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="d855c-106">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="d855c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d855c-107">Permissions</span></span>
<span data-ttu-id="d855c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d855c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d855c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d855c-110">Permission type</span></span>      | <span data-ttu-id="d855c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d855c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d855c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d855c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d855c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d855c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d855c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d855c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d855c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d855c-115">Not supported.</span></span>    |
|<span data-ttu-id="d855c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d855c-116">Application</span></span> | <span data-ttu-id="d855c-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d855c-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="d855c-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d855c-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d855c-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="d855c-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d855c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d855c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d855c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d855c-121">Optional query parameters</span></span>
<span data-ttu-id="d855c-122">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d855c-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d855c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d855c-123">Request headers</span></span>
| <span data-ttu-id="d855c-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d855c-124">Header</span></span>       | <span data-ttu-id="d855c-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d855c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d855c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d855c-126">Authorization</span></span>  | <span data-ttu-id="d855c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d855c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d855c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d855c-129">Request body</span></span>
<span data-ttu-id="d855c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d855c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d855c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d855c-131">Response</span></span>

<span data-ttu-id="d855c-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d855c-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d855c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d855c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d855c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d855c-134">Request</span></span>
<span data-ttu-id="d855c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d855c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="d855c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d855c-136">Response</span></span>
<span data-ttu-id="d855c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d855c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
