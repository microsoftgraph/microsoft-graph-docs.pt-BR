---
title: Criar uma equipe
description: Criar uma nova equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3e901225f5a8f94abb61a6b4052b0db2d47865c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519609"
---
# <a name="create-team"></a><span data-ttu-id="3a518-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="3a518-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a518-104">Criar uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3a518-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a518-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a518-105">Permissions</span></span>

<span data-ttu-id="3a518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a518-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a518-108">Permission type</span></span>                        | <span data-ttu-id="3a518-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a518-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3a518-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a518-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a518-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a518-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="3a518-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a518-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a518-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a518-113">Not supported.</span></span>                              |
| <span data-ttu-id="3a518-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a518-114">Application</span></span>                            | <span data-ttu-id="3a518-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a518-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3a518-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a518-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="3a518-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a518-117">Request headers</span></span>

| <span data-ttu-id="3a518-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a518-118">Header</span></span>        | <span data-ttu-id="3a518-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3a518-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="3a518-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a518-120">Authorization</span></span> | <span data-ttu-id="3a518-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a518-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a518-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a518-123">Content-Type</span></span>  | <span data-ttu-id="3a518-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a518-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="3a518-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a518-125">Request body</span></span>

<span data-ttu-id="3a518-126">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3a518-126">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3a518-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a518-127">Response</span></span>

<span data-ttu-id="3a518-128">Se bem-sucedida, essa API retornará uma resposta `202 Accepted` contendo um link para a [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3a518-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="3a518-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a518-129">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="3a518-130">Exemplo – permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="3a518-130">Example - delegated permissions</span></span>

<span data-ttu-id="3a518-131">Veja a seguir um exemplo de uma solicitação mínima.</span><span class="sxs-lookup"><span data-stu-id="3a518-131">Here is an example of a minimal request.</span></span> <span data-ttu-id="3a518-132">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="3a518-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="3a518-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a518-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="3a518-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a518-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="3a518-135">Exemplo – criar uma equipe com um aplicativo instalado, vários canais com guias fixadas usando permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="3a518-135">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="3a518-136">Aqui está a solicitação com um conteúdo completo.</span><span class="sxs-lookup"><span data-stu-id="3a518-136">Here is request with a full payload.</span></span> <span data-ttu-id="3a518-137">O cliente pode substituir os valores no modelo-base e adicionar itens com valor de matriz na máxima extensão permitida por regras de validação para a `specialization`.</span><span class="sxs-lookup"><span data-stu-id="3a518-137">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="3a518-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a518-138">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "visibility": "Private",
    "displayName": "Sample Engineering Team",
    "description": "This is a sample engineering team, used to showcase the range of properties supported by this API",
    "channels": [
        {
            "displayName": "Announcements 📢",
            "isFavoriteByDefault": true,
            "description": "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements."
        },
        {
            "displayName": "Training 🏋️",
            "isFavoriteByDefault": true,
            "description": "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
            "tabs": [
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
                    "name": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/en-us/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "name": "A Pinned YouTube Video",
                    "configuration": {
                        "contentUrl": "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
                        "websiteUrl": "https://www.youtube.com/watch?v=X8krAMdGvCQ"
                    }
                }
            ]
        },
        {
            "displayName": "Planning 📅 ",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
            "isFavoriteByDefault": false
        },
        {
            "displayName": "Issues and Feedback 🐞",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu."
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "Moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="3a518-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a518-139">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="3a518-140">Exemplo – permissões de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a518-140">Example - application permissions</span></span>

<span data-ttu-id="3a518-141">Aqui está um exemplo de uma solicitação mínima com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3a518-141">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="3a518-142">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="3a518-142">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="3a518-143">Ao emitir uma solicitação com permissões de aplicativo, um [usuário](../resources/user.md) deve ser especificado na coleção `owners`.</span><span class="sxs-lookup"><span data-stu-id="3a518-143">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="3a518-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a518-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="3a518-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a518-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="3a518-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="3a518-146">See also</span></span>

- [<span data-ttu-id="3a518-147">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="3a518-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/team-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
