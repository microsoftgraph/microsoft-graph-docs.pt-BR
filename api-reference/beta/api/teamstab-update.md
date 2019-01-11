---
title: Guia de atualização
description: Atualize as propriedades da guia especificada.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c17381432465ae318d86a818922d161ab46e762f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815061"
---
# <a name="update-tab"></a><span data-ttu-id="dbe70-103">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="dbe70-103">Update tab</span></span>

> <span data-ttu-id="dbe70-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbe70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbe70-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbe70-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbe70-106">Atualize as propriedades da [guia](../resources/teamstab.md)especificado. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="dbe70-106">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe70-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="dbe70-107">Permissions</span></span>
<span data-ttu-id="dbe70-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dbe70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbe70-110">Permission type</span></span>      | <span data-ttu-id="dbe70-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbe70-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbe70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbe70-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dbe70-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe70-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbe70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbe70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbe70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbe70-115">Not supported.</span></span>    |
|<span data-ttu-id="dbe70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbe70-116">Application</span></span>                            | <span data-ttu-id="dbe70-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe70-117">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="dbe70-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="dbe70-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dbe70-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="dbe70-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dbe70-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe70-120">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dbe70-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe70-121">Request headers</span></span>
| <span data-ttu-id="dbe70-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbe70-122">Header</span></span>       | <span data-ttu-id="dbe70-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dbe70-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dbe70-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbe70-124">Authorization</span></span>  | <span data-ttu-id="dbe70-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbe70-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dbe70-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbe70-127">Content-Type</span></span>  | <span data-ttu-id="dbe70-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dbe70-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbe70-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe70-129">Request body</span></span>
<span data-ttu-id="dbe70-130">No corpo da solicitação, fornece uma representação de JSON do objeto [tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="dbe70-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dbe70-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe70-131">Response</span></span>

<span data-ttu-id="dbe70-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dbe70-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dbe70-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbe70-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dbe70-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe70-134">Request</span></span>
<span data-ttu-id="dbe70-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbe70-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="dbe70-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe70-136">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dbe70-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="dbe70-137">See also</span></span>

[<span data-ttu-id="dbe70-138">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="dbe70-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
