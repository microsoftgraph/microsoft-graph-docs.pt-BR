---
title: Criar uma equipe
description: Criar uma nova equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 15eb03706a46d65f0b4e987042a943366ea6e944
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873410"
---
# <a name="create-team"></a><span data-ttu-id="ca9d7-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="ca9d7-103">Create team</span></span>

<span data-ttu-id="ca9d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca9d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca9d7-105">Criar uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca9d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca9d7-106">Permissions</span></span>

<span data-ttu-id="ca9d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca9d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca9d7-109">Permission type</span></span>                        | <span data-ttu-id="ca9d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca9d7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ca9d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca9d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca9d7-112">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca9d7-112">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="ca9d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca9d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca9d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-114">Not supported.</span></span>                              |
| <span data-ttu-id="ca9d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca9d7-115">Application</span></span>                            | <span data-ttu-id="ca9d7-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca9d7-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca9d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca9d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="ca9d7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-118">Request headers</span></span>

| <span data-ttu-id="ca9d7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca9d7-119">Header</span></span>        | <span data-ttu-id="ca9d7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ca9d7-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ca9d7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca9d7-121">Authorization</span></span> | <span data-ttu-id="ca9d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca9d7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca9d7-124">Content-Type</span></span>  | <span data-ttu-id="ca9d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca9d7-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ca9d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-126">Request body</span></span>

<span data-ttu-id="ca9d7-127">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-127">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca9d7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-128">Response</span></span>

<span data-ttu-id="ca9d7-129">Se bem-sucedida, essa API retornará uma resposta `202 Accepted` contendo um link para a [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-129">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="ca9d7-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca9d7-130">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="ca9d7-131">Exemplo 1: Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="ca9d7-131">Example 1: Delegated permissions</span></span>

<span data-ttu-id="ca9d7-132">Este é um exemplo de uma solicitação mínima.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-132">The following is an example of a minimal request.</span></span> <span data-ttu-id="ca9d7-133">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-133">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="ca9d7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_team_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```

##### <a name="response"></a><span data-ttu-id="ca9d7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-135">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="ca9d7-136">Exemplo 2: Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="ca9d7-136">Example 2: Application permissions</span></span>

<span data-ttu-id="ca9d7-137">Aqui está um exemplo de uma solicitação mínima usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-137">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="ca9d7-138">Ao omitir outras propriedades, o cliente está implicitamente obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-138">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="ca9d7-139">Ao emitir uma solicitação com permissões de aplicativo, um [usuário](../resources/user.md) deve ser especificado no conjunto `owners`.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-139">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="ca9d7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users('userId')"
  ]
}
```


#### <a name="response"></a><span data-ttu-id="ca9d7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-141">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_minimal",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="ca9d7-142">Exemplo 3: Criar uma equipe com vários canais, aplicativos instalados e guias fixadas usando permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="ca9d7-142">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="ca9d7-143">Aqui está uma solicitação com um conteúdo completo.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-143">The following is a request with a full payload.</span></span> <span data-ttu-id="ca9d7-144">O cliente pode substituir os valores no modelo-base e adicionar itens com valor de matriz na máxima extensão permitida por regras de validação para a `specialization`.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-144">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="ca9d7-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_team_post_full_payload"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
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
                        "contentUrl": "https://docs.microsoft.com/microsoftteams/microsoft-teams"
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
    "discoverySettings": {
        "showInTeamsSearchAndSuggestions": true
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


#### <a name="response"></a><span data-ttu-id="ca9d7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-146">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_full_payload",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="ca9d7-147">Exemplo 4: criar uma equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="ca9d7-147">Example 4: Create a team from group</span></span>

<span data-ttu-id="ca9d7-148">O exemplo a seguir mostra como você pode criar uma nova [equipe](../resources/team.md) a partir de um [grupo](../resources/group.md), dado um **groupId**.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-148">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="ca9d7-149">Observações sobre essa chamada:</span><span class="sxs-lookup"><span data-stu-id="ca9d7-149">A few thing to note about this call:</span></span>

* <span data-ttu-id="ca9d7-150">Para criar uma equipe, o grupo a partir do qual você a está criando deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-150">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="ca9d7-151">A equipe criada será sempre herdeira do nome de exibição, visibilidade, especialização e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-151">The team that's created will always inherit from the group's display name, visibility, specialization, and owners.</span></span> <span data-ttu-id="ca9d7-152">Portanto, ao fazer essa chamada com a propriedade **group@odata.bind**, a inclusão da equipe **displayName**, **visibilidade**, **especialização** ou propriedades **owners@odata.bind** retornarão um erro.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-152">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **owners@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="ca9d7-153">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-153">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="ca9d7-154">Recomendamos que você repita a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-154">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>


#### <a name="request"></a><span data-ttu-id="ca9d7-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-155">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
}
```


#### <a name="response"></a><span data-ttu-id="ca9d7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-156">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="ca9d7-157">Exemplo 5: Criar uma equipe a partir de um grupo com vários canais, aplicativos instalados e guias fixadas</span><span class="sxs-lookup"><span data-stu-id="ca9d7-157">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="ca9d7-158">A seguir está uma solicitação que converte um grupo existente com propriedades estendidas que criarão a equipe com vários canais, aplicativos instalados e guias fixadas.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-158">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="ca9d7-159">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-159">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="ca9d7-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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


#### <a name="response"></a><span data-ttu-id="ca9d7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-161">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="ca9d7-162">Exemplo 6: Criar uma equipe com um tipo de modelo de base não padrão</span><span class="sxs-lookup"><span data-stu-id="ca9d7-162">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="ca9d7-163">Os tipos de modelos base são modelos especiais criados pela Microsoft para setores específicos.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-163">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="ca9d7-164">Estes modelos base geralmente contêm aplicativos proprietários que não estão disponíveis nas lojas, e propriedade de equipe que ainda não tem suporte individual nos modelos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-164">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="ca9d7-165">Para criar uma equipe a partir de um modelo base não padrão, você vai precisar alterar a propriedade `template@odata.bind` no corpo da solicitação de `standard` para indicar o que você deseja criar para o modelo base padrão.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-165">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="ca9d7-166">Para saber mais sobre tipos de modelos base com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-166">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="ca9d7-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```

#### <a name="response"></a><span data-ttu-id="ca9d7-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-168">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="ca9d7-169">Exemplo 7: Criar uma equipe com um tipo de modelo base não padrão com propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="ca9d7-169">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="ca9d7-170">Os tipos de modelos base podem ser estendidos com propriedade adicionais, permitindo que você crie sobre um modelo base existente com configurações, canais, aplicativos ou guias de equipe adicionais.</span><span class="sxs-lookup"><span data-stu-id="ca9d7-170">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="ca9d7-171">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="ca9d7-171">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="ca9d7-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca9d7-172">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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

#### <a name="response"></a><span data-ttu-id="ca9d7-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca9d7-173">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard2",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

## <a name="see-also"></a><span data-ttu-id="ca9d7-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca9d7-174">See also</span></span>

- [<span data-ttu-id="ca9d7-175">Modelos disponíveis</span><span class="sxs-lookup"><span data-stu-id="ca9d7-175">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
- [<span data-ttu-id="ca9d7-176">Introdução aos modelos de Equipes de varejo</span><span class="sxs-lookup"><span data-stu-id="ca9d7-176">Getting started with Retail Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [<span data-ttu-id="ca9d7-177">Introdução aos modelos de Equipes médicas</span><span class="sxs-lookup"><span data-stu-id="ca9d7-177">Getting started with Healthcare Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [<span data-ttu-id="ca9d7-178">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="ca9d7-178">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
