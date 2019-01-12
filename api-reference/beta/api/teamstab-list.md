---
title: Guias de lista no canal
description: 'Recupere a lista das guias no canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 328c890f0bb585d5bdedd053dfc9206924b37334
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952829"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="ed77b-103">Guias de lista no canal</span><span class="sxs-lookup"><span data-stu-id="ed77b-103">List tabs in channel</span></span>

> <span data-ttu-id="ed77b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed77b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed77b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed77b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed77b-106">Recupere a lista das [guias](../resources/teamstab.md) no [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ed77b-106">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ed77b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed77b-107">Permissions</span></span>
<span data-ttu-id="ed77b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed77b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed77b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed77b-110">Permission type</span></span>      | <span data-ttu-id="ed77b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed77b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed77b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed77b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ed77b-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed77b-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="ed77b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed77b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed77b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed77b-115">Not supported.</span></span>    |
| <span data-ttu-id="ed77b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed77b-116">Application</span></span>                            | <span data-ttu-id="ed77b-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed77b-117">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="ed77b-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ed77b-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ed77b-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="ed77b-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ed77b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed77b-120">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed77b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed77b-121">Optional query parameters</span></span>

<span data-ttu-id="ed77b-122">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed77b-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed77b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed77b-123">Request headers</span></span>
| <span data-ttu-id="ed77b-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed77b-124">Header</span></span>       | <span data-ttu-id="ed77b-125">Valor</span><span class="sxs-lookup"><span data-stu-id="ed77b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed77b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed77b-126">Authorization</span></span>  | <span data-ttu-id="ed77b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed77b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed77b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed77b-129">Request body</span></span>
<span data-ttu-id="ed77b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed77b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed77b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed77b-131">Response</span></span>
<span data-ttu-id="ed77b-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [guias](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed77b-132">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed77b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed77b-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ed77b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed77b-134">Request</span></span>
<span data-ttu-id="ed77b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed77b-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="ed77b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed77b-136">Response</span></span>
<span data-ttu-id="ed77b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed77b-137">The following is an example of the response.</span></span>
><span data-ttu-id="ed77b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed77b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
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
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
