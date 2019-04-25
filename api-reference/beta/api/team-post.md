---
title: Criar uma equipe
description: Criar uma nova equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 394fa92f6ef97d6bc7a8dff0d4ddfe10c677bf99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536828"
---
# <a name="create-team"></a><span data-ttu-id="dc169-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="dc169-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc169-104">Criar uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="dc169-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc169-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc169-105">Permissions</span></span>

<span data-ttu-id="dc169-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc169-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc169-108">Permission type</span></span>                        | <span data-ttu-id="dc169-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc169-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dc169-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc169-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc169-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc169-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="dc169-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc169-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc169-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc169-113">Not supported.</span></span>                              |
| <span data-ttu-id="dc169-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc169-114">Application</span></span>                            | <span data-ttu-id="dc169-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc169-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dc169-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc169-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="dc169-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-117">Request headers</span></span>

| <span data-ttu-id="dc169-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc169-118">Header</span></span>        | <span data-ttu-id="dc169-119">Valor</span><span class="sxs-lookup"><span data-stu-id="dc169-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="dc169-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc169-120">Authorization</span></span> | <span data-ttu-id="dc169-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc169-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc169-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc169-123">Content-Type</span></span>  | <span data-ttu-id="dc169-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc169-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="dc169-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-125">Request body</span></span>

<span data-ttu-id="dc169-126">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="dc169-126">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dc169-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc169-127">Response</span></span>

<span data-ttu-id="dc169-128">Se bem-sucedida, essa API retornará uma resposta `202 Accepted` contendo um link para a [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="dc169-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="dc169-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc169-129">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="dc169-130">Exemplo 1: Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="dc169-130">Example 1: Delegated permissions</span></span>

<span data-ttu-id="dc169-131">Este é um exemplo de uma solicitação mínima.</span><span class="sxs-lookup"><span data-stu-id="dc169-131">The following is an example of a minimal request.</span></span> <span data-ttu-id="dc169-132">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="dc169-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="dc169-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```

##### <a name="response"></a><span data-ttu-id="dc169-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc169-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="dc169-135">Exemplo 2: Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="dc169-135">Example 2: Application permissions</span></span>

<span data-ttu-id="dc169-136">Aqui está um exemplo de uma solicitação mínima usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc169-136">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="dc169-137">Ao omitir outras propriedades, o cliente está implicitamente obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="dc169-137">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="dc169-138">Ao emitir uma solicitação com permissões de aplicativo, um [usuário](../resources/user.md) deve ser especificado no conjunto `owners`.</span><span class="sxs-lookup"><span data-stu-id="dc169-138">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="dc169-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-139">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="dc169-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc169-140">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-3-create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="dc169-141">Exemplo 3: Criar uma equipe com um aplicativo instalado, vários canais com guias fixadas usando permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="dc169-141">Example 3: Create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="dc169-142">Aqui está uma solicitação com um conteúdo completo.</span><span class="sxs-lookup"><span data-stu-id="dc169-142">The following is a request with a full payload.</span></span> <span data-ttu-id="dc169-143">O cliente pode substituir os valores no modelo-base e adicionar itens com valor de matriz na máxima extensão permitida por regras de validação para a `specialization`.</span><span class="sxs-lookup"><span data-stu-id="dc169-143">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span> 

#### <a name="request"></a><span data-ttu-id="dc169-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-144">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="dc169-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc169-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-4-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="dc169-146">Exemplo 4: Criar uma equipe com um tipo de modelo de base não padrão</span><span class="sxs-lookup"><span data-stu-id="dc169-146">Example 4: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="dc169-147">Os tipos de modelos base são modelos especiais criados pela Microsoft para setores específicos.</span><span class="sxs-lookup"><span data-stu-id="dc169-147">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="dc169-148">Estes modelos base geralmente contêm aplicativos proprietários que não estão disponíveis nas lojas, e propriedade de equipe que ainda não tem suporte individual nos modelos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dc169-148">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="dc169-149">Para criar uma equipe a partir de um modelo base não padrão, você vai precisar alterar a propriedade `template@odata.bind` no corpo da solicitação de `standard` para indicar o que você deseja criar para o modelo base padrão.</span><span class="sxs-lookup"><span data-stu-id="dc169-149">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="dc169-150">Para saber mais sobre tipos de modelos base com suporte, confira [Comece a trabalhar com modelos do Teams](https://docs.microsoft.com/pt-BR/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="dc169-150">To learn more about supported base template types, see [Get started with Teams templates](https://docs.microsoft.com/pt-BR/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="dc169-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-151">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```

#### <a name="response"></a><span data-ttu-id="dc169-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc169-152">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-5-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="dc169-153">Exemplo 5: Criar uma equipe com um tipo de modelo base não padrão com propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="dc169-153">Example 5: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="dc169-154">Os tipos de modelos base podem ser estendidos com propriedade adicionais, permitindo que você crie sobre um modelo base existente com configurações, canais, aplicativos ou guias de equipe adicionais.</span><span class="sxs-lookup"><span data-stu-id="dc169-154">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="dc169-155">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](https://docs.microsoft.com/pt-BR/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="dc169-155">To learn more about supported base template types and supported properties, see [Get started with Teams templates](https://docs.microsoft.com/pt-BR/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="dc169-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc169-156">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="dc169-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc169-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="dc169-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="dc169-158">See also</span></span>

- [<span data-ttu-id="dc169-159">Modelos disponíveis</span><span class="sxs-lookup"><span data-stu-id="dc169-159">Available templates</span></span>](https://docs.microsoft.com/pt-BR/MicrosoftTeams/get-started-with-teams-templates)
- [<span data-ttu-id="dc169-160">Introdução aos modelos de Equipes de varejo</span><span class="sxs-lookup"><span data-stu-id="dc169-160">Getting started with Retail Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [<span data-ttu-id="dc169-161">Introdução aos modelos de Equipes médicas</span><span class="sxs-lookup"><span data-stu-id="dc169-161">Getting started with Healthcare Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [<span data-ttu-id="dc169-162">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="dc169-162">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/api/team-post.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
