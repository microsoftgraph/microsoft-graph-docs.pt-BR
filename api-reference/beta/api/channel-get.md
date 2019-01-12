---
title: Obtenha o canal
description: Recupere as propriedades e relacionamentos de um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bd02ce2e46dc176ee9c94f0f20c880e278efe5f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966360"
---
# <a name="get-channel"></a><span data-ttu-id="3fa3a-103">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="3fa3a-103">Get channel</span></span>

> <span data-ttu-id="3fa3a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fa3a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3fa3a-106">Recupere as propriedades e relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="3fa3a-106">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa3a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3fa3a-107">Permissions</span></span>
<span data-ttu-id="3fa3a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa3a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fa3a-110">Permission type</span></span>      | <span data-ttu-id="3fa3a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fa3a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fa3a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fa3a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3fa3a-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa3a-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3fa3a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fa3a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fa3a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-115">Not supported.</span></span>    |
|<span data-ttu-id="3fa3a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fa3a-116">Application</span></span> | <span data-ttu-id="3fa3a-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa3a-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="3fa3a-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3fa3a-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3fa3a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa3a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fa3a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3fa3a-121">Optional query parameters</span></span>

<span data-ttu-id="3fa3a-122">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fa3a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fa3a-123">Request headers</span></span>
| <span data-ttu-id="3fa3a-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fa3a-124">Header</span></span>       | <span data-ttu-id="3fa3a-125">Valor</span><span class="sxs-lookup"><span data-stu-id="3fa3a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3fa3a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fa3a-126">Authorization</span></span>  | <span data-ttu-id="3fa3a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fa3a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fa3a-129">Request body</span></span>
<span data-ttu-id="3fa3a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fa3a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fa3a-131">Response</span></span>

<span data-ttu-id="3fa3a-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fa3a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fa3a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fa3a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fa3a-134">Request</span></span>
<span data-ttu-id="3fa3a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="3fa3a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fa3a-136">Response</span></span>
<span data-ttu-id="3fa3a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-137">Here is an example of the response.</span></span> 

><span data-ttu-id="3fa3a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fa3a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
