---
title: Crie uma equipe
description: Crie uma nova equipe.
author: nkramer
ms.openlocfilehash: c77ca5ab76640c9c310b628f4eee106e7443fee7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362836"
---
# <a name="create-team"></a><span data-ttu-id="db266-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="db266-103">Create team</span></span>

> <span data-ttu-id="db266-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db266-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db266-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db266-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db266-106">Crie uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="db266-106">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db266-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="db266-107">Permissions</span></span>

<span data-ttu-id="db266-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db266-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db266-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db266-110">Permission type</span></span>                        | <span data-ttu-id="db266-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db266-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="db266-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db266-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="db266-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db266-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="db266-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db266-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db266-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db266-115">Not supported.</span></span>                              |
| <span data-ttu-id="db266-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db266-116">Application</span></span>                            | <span data-ttu-id="db266-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db266-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="db266-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db266-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="db266-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db266-119">Request headers</span></span>

| <span data-ttu-id="db266-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db266-120">Header</span></span>        | <span data-ttu-id="db266-121">Valor</span><span class="sxs-lookup"><span data-stu-id="db266-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="db266-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db266-122">Authorization</span></span> | <span data-ttu-id="db266-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db266-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db266-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db266-125">Content-Type</span></span>  | <span data-ttu-id="db266-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db266-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="db266-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db266-127">Request body</span></span>

<span data-ttu-id="db266-128">No corpo da solicitação, fornece uma representação JSON de um objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="db266-128">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db266-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="db266-129">Response</span></span>

<span data-ttu-id="db266-130">Se tiver êxito, essa API retornará um `202 Accepted` resposta contendo um link para o [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="db266-130">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="db266-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db266-131">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="db266-132">Exemplo - permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="db266-132">Example - delegated permissions</span></span>

<span data-ttu-id="db266-133">Aqui está um exemplo de uma solicitação mínimo.</span><span class="sxs-lookup"><span data-stu-id="db266-133">Here is an example of a minimal request.</span></span> <span data-ttu-id="db266-134">Omitindo outras propriedades, o cliente está demorando implicitamente padrões do modelo pré-definidos representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="db266-134">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="db266-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db266-135">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="db266-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="db266-136">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="db266-137">Exemplo - criar uma equipe com um aplicativo instalado, vários canais com guias fixados usando delegada permissões</span><span class="sxs-lookup"><span data-stu-id="db266-137">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="db266-138">Aqui está uma solicitação com uma carga completa.</span><span class="sxs-lookup"><span data-stu-id="db266-138">Here is request with a full payload.</span></span> <span data-ttu-id="db266-139">O cliente pode substituir os valores no modelo base e adicionar a itens de valor matriz até os limites permitidos por regras de validação para o `specialization`.</span><span class="sxs-lookup"><span data-stu-id="db266-139">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="db266-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db266-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="db266-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="db266-141">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="db266-142">Exemplo - permissões de aplicativo</span><span class="sxs-lookup"><span data-stu-id="db266-142">Example - application permissions</span></span>

<span data-ttu-id="db266-143">Aqui está um exemplo de uma solicitação mínimo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db266-143">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="db266-144">Omitindo outras propriedades, o cliente está demorando implicitamente padrões do modelo pré-definidos representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="db266-144">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="db266-145">Quando a emitindo uma solicitação com permissões de aplicativo um [usuário](../resources/user.md) deve ser especificado no `owners` conjunto.</span><span class="sxs-lookup"><span data-stu-id="db266-145">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="db266-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db266-146">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="db266-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="db266-147">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="db266-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="db266-148">See also</span></span>

- [<span data-ttu-id="db266-149">Criando um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="db266-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
