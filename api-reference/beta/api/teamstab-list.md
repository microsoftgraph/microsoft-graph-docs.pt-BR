---
title: Listar guias no canal
description: 'Recupere a lista de guias no canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5dc85d521c4cbf29ca3844937ceb04a7a980706a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537010"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="5bfc1-103">Listar guias no canal</span><span class="sxs-lookup"><span data-stu-id="5bfc1-103">List tabs in channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bfc1-104">Recupere a lista de [guias](../resources/teamstab.md) no [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="5bfc1-104">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="5bfc1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bfc1-105">Permissions</span></span>
<span data-ttu-id="5bfc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bfc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bfc1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bfc1-108">Permission type</span></span>      | <span data-ttu-id="5bfc1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bfc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bfc1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bfc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bfc1-111">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="5bfc1-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="5bfc1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bfc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bfc1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-113">Not supported.</span></span>    |
| <span data-ttu-id="5bfc1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bfc1-114">Application</span></span>                            | <span data-ttu-id="5bfc1-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bfc1-115">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="5bfc1-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5bfc1-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5bfc1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfc1-118">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bfc1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5bfc1-119">Optional query parameters</span></span>

<span data-ttu-id="5bfc1-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bfc1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfc1-121">Request headers</span></span>
| <span data-ttu-id="5bfc1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bfc1-122">Header</span></span>       | <span data-ttu-id="5bfc1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5bfc1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5bfc1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bfc1-124">Authorization</span></span>  | <span data-ttu-id="5bfc1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5bfc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfc1-127">Request body</span></span>
<span data-ttu-id="5bfc1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bfc1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfc1-129">Response</span></span>
<span data-ttu-id="5bfc1-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Tabs](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bfc1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bfc1-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5bfc1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfc1-132">Request</span></span>
<span data-ttu-id="5bfc1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs?$expand=teamsApp
```

#### <a name="response"></a><span data-ttu-id="5bfc1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfc1-134">Response</span></span>
<span data-ttu-id="5bfc1-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-135">The following is an example of the response.</span></span>
><span data-ttu-id="5bfc1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bfc1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
