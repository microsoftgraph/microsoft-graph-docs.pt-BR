---
title: Listar guias no canal
description: 'Recupere a lista de guias no canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d70fc12e64d056cd484502d46bd25874951f79a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509255"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="571a7-103">Listar guias no canal</span><span class="sxs-lookup"><span data-stu-id="571a7-103">List tabs in channel</span></span>

<span data-ttu-id="571a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="571a7-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="571a7-105">Recupere a lista de [guias](../resources/teamstab.md) no [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="571a7-105">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="571a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="571a7-106">Permissions</span></span>
<span data-ttu-id="571a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="571a7-109">Permission type</span></span>      | <span data-ttu-id="571a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="571a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="571a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="571a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="571a7-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="571a7-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="571a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="571a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="571a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="571a7-114">Not supported.</span></span>    |
| <span data-ttu-id="571a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="571a7-115">Application</span></span>                            | <span data-ttu-id="571a7-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="571a7-116">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="571a7-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="571a7-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="571a7-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="571a7-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="571a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="571a7-119">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="571a7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="571a7-120">Optional query parameters</span></span>

<span data-ttu-id="571a7-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="571a7-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="571a7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="571a7-122">Request headers</span></span>
| <span data-ttu-id="571a7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="571a7-123">Header</span></span>       | <span data-ttu-id="571a7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="571a7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="571a7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="571a7-125">Authorization</span></span>  | <span data-ttu-id="571a7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="571a7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="571a7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="571a7-128">Request body</span></span>
<span data-ttu-id="571a7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="571a7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="571a7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="571a7-130">Response</span></span>
<span data-ttu-id="571a7-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Tabs](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="571a7-131">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571a7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="571a7-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="571a7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="571a7-133">Request</span></span>
<span data-ttu-id="571a7-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="571a7-134">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs?$expand=teamsApp
```

#### <a name="response"></a><span data-ttu-id="571a7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="571a7-135">Response</span></span>
<span data-ttu-id="571a7-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="571a7-136">The following is an example of the response.</span></span>
><span data-ttu-id="571a7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="571a7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": "20",
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
