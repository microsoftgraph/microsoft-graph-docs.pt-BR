---
title: Atualizar guia
description: Atualiza as propriedades da guia especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bdfcc21c0e078c20b04db2e9d5cce6247ac86aeb
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848332"
---
# <a name="update-tab"></a><span data-ttu-id="abc4d-103">Atualizar guia</span><span class="sxs-lookup"><span data-stu-id="abc4d-103">Update tab</span></span>

<span data-ttu-id="abc4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc4d-105">Atualiza as propriedades da [guia](../resources/teamstab.md)especificada. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="abc4d-105">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="abc4d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="abc4d-106">Permissions</span></span>
<span data-ttu-id="abc4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="abc4d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abc4d-109">Permission type</span></span>      | <span data-ttu-id="abc4d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abc4d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abc4d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abc4d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="abc4d-112">TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="abc4d-112">TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="abc4d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abc4d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abc4d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abc4d-114">Not supported.</span></span>    |
|<span data-ttu-id="abc4d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abc4d-115">Application</span></span>                            | <span data-ttu-id="abc4d-116">TeamsTab. ReadWrite. Group \*, TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="abc4d-116">TeamsTab.ReadWrite.Group\*, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="abc4d-117">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="abc4d-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="abc4d-118">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="abc4d-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="abc4d-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="abc4d-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="abc4d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abc4d-120">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="abc4d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abc4d-121">Request headers</span></span>
| <span data-ttu-id="abc4d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abc4d-122">Header</span></span>       | <span data-ttu-id="abc4d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="abc4d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abc4d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="abc4d-124">Authorization</span></span>  | <span data-ttu-id="abc4d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abc4d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="abc4d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abc4d-127">Content-Type</span></span>  | <span data-ttu-id="abc4d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="abc4d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abc4d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abc4d-129">Request body</span></span>
<span data-ttu-id="abc4d-130">No corpo da solicitação, forneça uma representação JSON do objeto [Tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="abc4d-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="abc4d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc4d-131">Response</span></span>

<span data-ttu-id="abc4d-132">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="abc4d-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="abc4d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abc4d-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="abc4d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abc4d-134">Request</span></span>
<span data-ttu-id="abc4d-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="abc4d-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="abc4d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc4d-136">Response</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="abc4d-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="abc4d-137">See also</span></span>

[<span data-ttu-id="abc4d-138">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="abc4d-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


