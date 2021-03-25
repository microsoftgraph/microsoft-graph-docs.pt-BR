---
title: Criar equipe
description: Criar uma nova equipe.
author: anandjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a6a26b350f27d81d9a5ae0d5279bf62058fa161
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202636"
---
# <a name="create-team"></a><span data-ttu-id="48a71-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="48a71-103">Create team</span></span>

<span data-ttu-id="48a71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48a71-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48a71-105">Criar uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="48a71-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48a71-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="48a71-106">Permissions</span></span>

<span data-ttu-id="48a71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48a71-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48a71-109">Permission type</span></span>                        | <span data-ttu-id="48a71-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48a71-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="48a71-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48a71-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48a71-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a71-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="48a71-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48a71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48a71-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48a71-114">Not supported.</span></span>                              |
| <span data-ttu-id="48a71-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48a71-115">Application</span></span>                            | <span data-ttu-id="48a71-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a71-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="48a71-117">**Observação**: A permissão Teamwork.Migrate.All é *somente* suportado para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="48a71-117">**Note**: The Teamwork.Migrate.All permission is *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="48a71-118">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="48a71-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="48a71-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="48a71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-120">Request headers</span></span>

| <span data-ttu-id="48a71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48a71-121">Header</span></span>        | <span data-ttu-id="48a71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="48a71-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="48a71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48a71-123">Authorization</span></span> | <span data-ttu-id="48a71-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48a71-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48a71-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48a71-126">Content-Type</span></span>  | <span data-ttu-id="48a71-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48a71-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48a71-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-129">Request body</span></span>

<span data-ttu-id="48a71-130">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="48a71-130">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48a71-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-131">Response</span></span>

<span data-ttu-id="48a71-132">Se bem-sucedida, essa API retornará uma resposta `202 Accepted` contendo um link para a [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="48a71-132">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="48a71-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48a71-133">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="48a71-134">Exemplo 1: Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="48a71-134">Example 1: Delegated permissions</span></span>

<span data-ttu-id="48a71-135">Este é um exemplo de uma solicitação mínima.</span><span class="sxs-lookup"><span data-stu-id="48a71-135">The following is an example of a minimal request.</span></span> <span data-ttu-id="48a71-136">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="48a71-136">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="48a71-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-138">HTTP</span></span>](#tab/http)
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


---


##### <a name="response"></a><span data-ttu-id="48a71-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-139">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="48a71-140">Exemplo 2: Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="48a71-140">Example 2: Application permissions</span></span>

<span data-ttu-id="48a71-141">Aqui está um exemplo de uma solicitação mínima usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48a71-141">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="48a71-142">Ao omitir outras propriedades, o cliente está implicitamente obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="48a71-142">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="48a71-143">Ao emitir uma solicitação com permissões de aplicativo, um [usuário](../resources/user.md) deve ser especificado no conjunto `members`.</span><span class="sxs-lookup"><span data-stu-id="48a71-143">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `members` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="48a71-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   "displayName":"My Sample Team",
   "description":"My Sample Team’s Description",
   "members":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "roles":[
            "owner"
         ],
         "user@odata.bind":"https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')"
      }
   ]
}
```


---


#### <a name="response"></a><span data-ttu-id="48a71-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-146">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_minimal",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="48a71-147">Exemplo 3: Criar uma equipe com vários canais, aplicativos instalados e guias fixadas usando permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="48a71-147">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="48a71-148">Aqui está uma solicitação com um conteúdo completo.</span><span class="sxs-lookup"><span data-stu-id="48a71-148">The following is a request with a full payload.</span></span> <span data-ttu-id="48a71-149">O cliente pode substituir os valores no modelo-base e adicionar itens com valor de matriz na máxima extensão permitida por regras de validação para a `specialization`.</span><span class="sxs-lookup"><span data-stu-id="48a71-149">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a71-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-151">HTTP</span></span>](#tab/http)
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
                    "displayName": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "displayName": "A Pinned YouTube Video",
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
---

#### <a name="response"></a><span data-ttu-id="48a71-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-152">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_full_payload",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('958e8cf8-169a-42aa-8599-5c1c5479c0ca')/operations('00000000-0000-0000-0000-000000000000')
Content-Location: /teams('958e8cf8-169a-42aa-8599-5c1c5479c0ca')
Content-Length: 0
```

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="48a71-153">Exemplo 4: criar uma equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="48a71-153">Example 4: Create a team from group</span></span>

<span data-ttu-id="48a71-154">O exemplo a seguir mostra como você pode criar uma nova [equipe](../resources/team.md) a partir de um [grupo](../resources/group.md), dado um **groupId**.</span><span class="sxs-lookup"><span data-stu-id="48a71-154">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="48a71-155">Observações sobre essa chamada:</span><span class="sxs-lookup"><span data-stu-id="48a71-155">A few things to note about this call:</span></span>

* <span data-ttu-id="48a71-156">Para criar uma equipe, o grupo a partir do qual você a está criando deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="48a71-156">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="48a71-157">A equipe criada será sempre herdeira do nome de exibição, visibilidade, especialização e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="48a71-157">The team that's created will always inherit from the group's display name, visibility, specialization, and members.</span></span> <span data-ttu-id="48a71-158">Portanto, ao tomar essa decisão com a propriedade **group@odata.bind**, a inclusão da equipe **displayName**, **visibilidade**, **especialização** ou propriedades **owners@odata.bind** retornarão um erro.</span><span class="sxs-lookup"><span data-stu-id="48a71-158">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **members@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="48a71-159">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="48a71-159">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="48a71-160">Recomendamos que você repita a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="48a71-160">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a71-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
}
```

---

---
#### <a name="response"></a><span data-ttu-id="48a71-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-163">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('71392b2f-1765-406e-86af-5907d9bdb2ab')/operations('9698b2b8-9636-4f49-b7a8-10dadfa7062a')
Content-Location: /teams('71392b2f-1765-406e-86af-5907d9bdb2ab')
Content-Length: 0
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="48a71-164">Exemplo 5: Criar uma equipe a partir de um grupo com vários canais, aplicativos instalados e guias fixadas</span><span class="sxs-lookup"><span data-stu-id="48a71-164">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="48a71-165">A seguir está uma solicitação que converte um grupo existente com propriedades estendidas que criarão a equipe com vários canais, aplicativos instalados e guias fixadas.</span><span class="sxs-lookup"><span data-stu-id="48a71-165">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="48a71-166">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="48a71-166">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a71-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   "group@odata.bind":"https://graph.microsoft.com/v1.0/groups('dbd8de4f-5d47-48da-87f1-594bed003375')",
   "channels":[
      {
         "displayName":"Class Announcements 📢",
         "isFavoriteByDefault":true
      },
      {
         "displayName":"Homework 🏋️",
         "isFavoriteByDefault":true
      }
   ],
   "memberSettings":{
      "allowCreateUpdateChannels":false,
      "allowDeleteChannels":false,
      "allowAddRemoveApps":false,
      "allowCreateUpdateRemoveTabs":false,
      "allowCreateUpdateRemoveConnectors":false
   },
   "installedApps":[
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
}
```


---

---
#### <a name="response"></a><span data-ttu-id="48a71-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-169">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="48a71-170">Exemplo 6: Criar uma equipe com um tipo de modelo de base não padrão</span><span class="sxs-lookup"><span data-stu-id="48a71-170">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="48a71-171">Os tipos de modelos base são modelos especiais criados pela Microsoft para setores específicos.</span><span class="sxs-lookup"><span data-stu-id="48a71-171">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="48a71-172">Estes modelos base geralmente contêm aplicativos proprietários que não estão disponíveis nas lojas, e propriedade de equipe que ainda não tem suporte individual nos modelos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="48a71-172">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="48a71-173">Para criar uma equipe a partir de um modelo base não padrão, você vai precisar alterar a propriedade `template@odata.bind` no corpo da solicitação de `standard` para indicar o que você deseja criar para o modelo base padrão.</span><span class="sxs-lookup"><span data-stu-id="48a71-173">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="48a71-174">Para saber mais sobre tipos de modelos base com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="48a71-174">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-175">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a71-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```


---

---

#### <a name="response"></a><span data-ttu-id="48a71-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-177">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="48a71-178">Exemplo 7: Criar uma equipe com um tipo de modelo base não padrão com propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="48a71-178">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="48a71-179">Os tipos de modelos base podem ser estendidos com propriedade adicionais, permitindo que você crie sobre um modelo base existente com configurações, canais, aplicativos ou guias de equipe adicionais.</span><span class="sxs-lookup"><span data-stu-id="48a71-179">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="48a71-180">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="48a71-180">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-181">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a71-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a71-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
   "displayName":"My Class Team",
   "description":"My Class Team’s Description",
   "channels":[
      {
         "displayName":"Class Announcements 📢",
         "isFavoriteByDefault":true
      },
      {
         "displayName":"Homework 🏋️",
         "isFavoriteByDefault":true
      }
   ],
   "memberSettings":{
      "allowCreateUpdateChannels":false,
      "allowDeleteChannels":false,
      "allowAddRemoveApps":false,
      "allowCreateUpdateRemoveTabs":false,
      "allowCreateUpdateRemoveConnectors":false
   },
   "installedApps":[
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
}
```


---

---
#### <a name="response"></a><span data-ttu-id="48a71-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-183">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard2",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-8-create-a-team-in-migration-mode"></a><span data-ttu-id="48a71-184">Exemplo 8: Criar uma equipe no modo de migração</span><span class="sxs-lookup"><span data-stu-id="48a71-184">Example 8: Create a team in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="48a71-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48a71-185">Request</span></span>

<span data-ttu-id="48a71-186">O exemplo a seguir mostra como criar uma equipe para mensagens importadas.</span><span class="sxs-lookup"><span data-stu-id="48a71-186">The following example shows how to create a team for imported messages.</span></span>

><span data-ttu-id="48a71-187">**Observação:** No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="48a71-187">**Note:** In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.|</span></span>

><span data-ttu-id="48a71-188">**Observação:** Equipes criadas no modo de migração só suportam o modelo `standard`.</span><span class="sxs-lookup"><span data-stu-id="48a71-188">**Note:** Teams created in migration mode only support the `standard` template.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "@microsoft.graph.teamCreationMode": "migration",
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="48a71-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="48a71-189">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
```

#### <a name="error-response"></a><span data-ttu-id="48a71-190">Resposta de erro</span><span class="sxs-lookup"><span data-stu-id="48a71-190">Error response</span></span>

<span data-ttu-id="48a71-191">Se a solicitação não for bem-sucedida, este método retorna um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="48a71-191">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> 

```http
400 Bad Request
```

<span data-ttu-id="48a71-192">Os seguintes são motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="48a71-192">The following are common reasons for this response:</span></span>

* <span data-ttu-id="48a71-193">**createdDateTime** é definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="48a71-193">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="48a71-194">**createdDateTime** está especificado corretamente, mas o atributo da instância **teamCreationMode** está ausente ou definido com um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="48a71-194">**createdDateTime** is correctly specified but the **teamCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="see-also"></a><span data-ttu-id="48a71-195">Confira também</span><span class="sxs-lookup"><span data-stu-id="48a71-195">See also</span></span>

* [<span data-ttu-id="48a71-196">Migração completa para uma equipe</span><span class="sxs-lookup"><span data-stu-id="48a71-196">Complete migration for a team</span></span>](team-completemigration.md)
* [<span data-ttu-id="48a71-197">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="48a71-197">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="48a71-198">Create channel</span><span class="sxs-lookup"><span data-stu-id="48a71-198">Create channel</span></span>](channel-post.md)
* [<span data-ttu-id="48a71-199">Modelos disponíveis</span><span class="sxs-lookup"><span data-stu-id="48a71-199">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
* [<span data-ttu-id="48a71-200">Introdução aos modelos de Equipes de varejo</span><span class="sxs-lookup"><span data-stu-id="48a71-200">Getting started with Retail Teams templates</span></span>](/MicrosoftTeams/get-started-with-retail-teams-templates)
* [<span data-ttu-id="48a71-201">Introdução aos modelos de Equipes médicas</span><span class="sxs-lookup"><span data-stu-id="48a71-201">Getting started with Healthcare Teams templates</span></span>](/MicrosoftTeams/healthcare/healthcare-templates)
* [<span data-ttu-id="48a71-202">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="48a71-202">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
