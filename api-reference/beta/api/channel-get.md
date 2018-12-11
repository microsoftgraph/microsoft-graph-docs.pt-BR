---
title: Obtenha o canal
description: Recupere as propriedades e relacionamentos de um canal.
ms.openlocfilehash: a25f97c456ec92bfa1d15974d42698f6968b6338
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222412"
---
# <a name="get-channel"></a><span data-ttu-id="86475-103">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="86475-103">Get channel</span></span>

> <span data-ttu-id="86475-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="86475-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86475-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86475-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86475-106">Recupere as propriedades e relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="86475-106">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86475-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="86475-107">Permissions</span></span>
<span data-ttu-id="86475-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86475-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86475-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86475-110">Permission type</span></span>      | <span data-ttu-id="86475-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86475-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86475-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86475-112">Delegated (work or school account)</span></span> | <span data-ttu-id="86475-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86475-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86475-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86475-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86475-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86475-115">Not supported.</span></span>    |
|<span data-ttu-id="86475-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86475-116">Application</span></span> | <span data-ttu-id="86475-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86475-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="86475-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="86475-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="86475-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="86475-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="86475-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86475-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="86475-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86475-121">Optional query parameters</span></span>

<span data-ttu-id="86475-122">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86475-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86475-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86475-123">Request headers</span></span>
| <span data-ttu-id="86475-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86475-124">Header</span></span>       | <span data-ttu-id="86475-125">Valor</span><span class="sxs-lookup"><span data-stu-id="86475-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86475-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="86475-126">Authorization</span></span>  | <span data-ttu-id="86475-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86475-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86475-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86475-129">Request body</span></span>
<span data-ttu-id="86475-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86475-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86475-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="86475-131">Response</span></span>

<span data-ttu-id="86475-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86475-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86475-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86475-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86475-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86475-134">Request</span></span>
<span data-ttu-id="86475-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86475-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="86475-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="86475-136">Response</span></span>
<span data-ttu-id="86475-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86475-137">Here is an example of the response.</span></span> 

><span data-ttu-id="86475-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86475-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
