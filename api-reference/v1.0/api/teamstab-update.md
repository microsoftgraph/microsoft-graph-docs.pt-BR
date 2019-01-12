---
title: Guia de atualização
description: Atualize as propriedades da guia especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f7bb00fb58513c32c66f72a9ef852e799674a52e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944702"
---
# <a name="update-tab"></a><span data-ttu-id="8bb7b-103">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="8bb7b-103">Update tab</span></span>



<span data-ttu-id="8bb7b-104">Atualize as propriedades da [guia](../resources/teamstab.md)especificado. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb7b-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8bb7b-105">Permissions</span></span>
<span data-ttu-id="8bb7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8bb7b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bb7b-108">Permission type</span></span>      | <span data-ttu-id="8bb7b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bb7b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bb7b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bb7b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bb7b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb7b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bb7b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bb7b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb7b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-113">Not supported.</span></span>    |
|<span data-ttu-id="8bb7b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bb7b-114">Application</span></span>                            | <span data-ttu-id="8bb7b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb7b-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="8bb7b-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8bb7b-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8bb7b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb7b-118">HTTP request</span></span>

```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bb7b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb7b-119">Request headers</span></span>
| <span data-ttu-id="8bb7b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bb7b-120">Header</span></span>       | <span data-ttu-id="8bb7b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8bb7b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8bb7b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bb7b-122">Authorization</span></span>  | <span data-ttu-id="8bb7b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8bb7b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bb7b-125">Content-Type</span></span>  | <span data-ttu-id="8bb7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb7b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8bb7b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb7b-127">Request body</span></span>
<span data-ttu-id="8bb7b-128">No corpo da solicitação, fornece uma representação de JSON do objeto [tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="8bb7b-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8bb7b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb7b-129">Response</span></span>

<span data-ttu-id="8bb7b-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8bb7b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bb7b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8bb7b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bb7b-132">Request</span></span>
<span data-ttu-id="8bb7b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bb7b-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="8bb7b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bb7b-134">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="8bb7b-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="8bb7b-135">See also</span></span>

[<span data-ttu-id="8bb7b-136">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="8bb7b-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
