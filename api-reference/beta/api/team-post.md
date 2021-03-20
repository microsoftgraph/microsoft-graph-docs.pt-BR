---
title: Criar equipe
description: Criar uma nova equipe.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d596d39330ecf332313ca0d82766c71d977980c0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942255"
---
# <a name="create-team"></a><span data-ttu-id="7a977-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="7a977-103">Create team</span></span>

<span data-ttu-id="7a977-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a977-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a977-105">Criar uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7a977-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a977-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a977-106">Permissions</span></span>

<span data-ttu-id="7a977-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a977-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a977-109">Permission type</span></span>                        | <span data-ttu-id="7a977-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a977-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7a977-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a977-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a977-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a977-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7a977-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a977-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a977-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a977-114">Not supported.</span></span>                              |
| <span data-ttu-id="7a977-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a977-115">Application</span></span>                            | <span data-ttu-id="7a977-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a977-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="7a977-117">**Observação**: A permissão Teamwork.Migrate.All é *somente* suportado para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="7a977-117">**Note**: The Teamwork.Migrate.All permission is *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="7a977-118">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="7a977-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="7a977-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="7a977-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-120">Request headers</span></span>

| <span data-ttu-id="7a977-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a977-121">Header</span></span>        | <span data-ttu-id="7a977-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a977-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7a977-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a977-123">Authorization</span></span> | <span data-ttu-id="7a977-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a977-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a977-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a977-126">Content-Type</span></span>  | <span data-ttu-id="7a977-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a977-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a977-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-129">Request body</span></span>

<span data-ttu-id="7a977-130">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7a977-130">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7a977-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-131">Response</span></span>

<span data-ttu-id="7a977-132">Se bem-sucedida, essa API retornará uma resposta `202 Accepted` contendo um link para a [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="7a977-132">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="7a977-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a977-133">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="7a977-134">Exemplo 1: Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="7a977-134">Example 1: Delegated permissions</span></span>

<span data-ttu-id="7a977-135">Este é um exemplo de uma solicitação mínima.</span><span class="sxs-lookup"><span data-stu-id="7a977-135">The following is an example of a minimal request.</span></span> <span data-ttu-id="7a977-136">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="7a977-136">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a977-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="7a977-139">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-142">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->

##### <a name="response"></a><span data-ttu-id="7a977-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-143">Response</span></span>

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

### <a name="example-2-application-permissions"></a><span data-ttu-id="7a977-144">Exemplo 2: Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="7a977-144">Example 2: Application permissions</span></span>

<span data-ttu-id="7a977-145">Aqui está um exemplo de uma solicitação mínima usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a977-145">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="7a977-146">Ao omitir outras propriedades, o cliente está implicitamente obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="7a977-146">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="7a977-147">Ao emitir uma solicitação com permissões de aplicativo, um [usuário](../resources/user.md) deve ser especificado no conjunto `members`.</span><span class="sxs-lookup"><span data-stu-id="7a977-147">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `members` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-148">Request</span></span>
<!-- markdownlint-disable MD025 -->

# <a name="http"></a>[<span data-ttu-id="7a977-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('standard')",
   "displayName":"My Sample Team",
   "description":"My Sample Team’s Description",
   "members":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "roles":[
            "owner"
         ],
         "user@odata.bind":"https://graph.microsoft.com/beta/users('0040b377-61d8-43db-94f5-81374122dc7e')"
      }
   ]
}
```

# <a name="c"></a>[<span data-ttu-id="7a977-150">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-153">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a977-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-154">Response</span></span>
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

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="7a977-155">Exemplo 3: Criar uma equipe com vários canais, aplicativos instalados e guias fixadas usando permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="7a977-155">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="7a977-156">Aqui está uma solicitação com um conteúdo completo.</span><span class="sxs-lookup"><span data-stu-id="7a977-156">The following is a request with a full payload.</span></span> <span data-ttu-id="7a977-157">O cliente pode substituir os valores no modelo-base e adicionar itens com valor de matriz na máxima extensão permitida por regras de validação para a `specialization`.</span><span class="sxs-lookup"><span data-stu-id="7a977-157">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-158">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a977-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_full_payload"
}-->

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
# <a name="c"></a>[<span data-ttu-id="7a977-160">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-full-payload-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-full-payload-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-full-payload-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-163">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-full-payload-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a977-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-164">Response</span></span>
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

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="7a977-165">Exemplo 4: criar uma equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="7a977-165">Example 4: Create a team from group</span></span>

<span data-ttu-id="7a977-166">O exemplo a seguir mostra como você pode criar uma nova [equipe](../resources/team.md) a partir de um [grupo](../resources/group.md), dado um **groupId**.</span><span class="sxs-lookup"><span data-stu-id="7a977-166">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="7a977-167">Observações sobre essa chamada:</span><span class="sxs-lookup"><span data-stu-id="7a977-167">A few things to note about this call:</span></span>

* <span data-ttu-id="7a977-168">Para criar uma equipe, o grupo a partir do qual você a está criando deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="7a977-168">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="7a977-169">A equipe criada será sempre herdeira do nome de exibição, visibilidade, especialização e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="7a977-169">The team that's created will always inherit from the group's display name, visibility, specialization, and members.</span></span> <span data-ttu-id="7a977-170">Portanto, ao tomar essa decisão com a propriedade **group@odata.bind**, a inclusão da equipe **displayName**, **visibilidade**, **especialização** ou propriedades **owners@odata.bind** retornarão um erro.</span><span class="sxs-lookup"><span data-stu-id="7a977-170">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **members@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="7a977-171">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="7a977-171">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="7a977-172">Recomendamos que você repita a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="7a977-172">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a977-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-174">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="7a977-175">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-178">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a977-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-179">Response</span></span>
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

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="7a977-180">Exemplo 5: Criar uma equipe a partir de um grupo com vários canais, aplicativos instalados e guias fixadas</span><span class="sxs-lookup"><span data-stu-id="7a977-180">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="7a977-181">A seguir está uma solicitação que converte um grupo existente com propriedades estendidas que criarão a equipe com vários canais, aplicativos instalados e guias fixadas.</span><span class="sxs-lookup"><span data-stu-id="7a977-181">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="7a977-182">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="7a977-182">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-183">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a977-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('standard')",
   "group@odata.bind":"https://graph.microsoft.com/v1.0/groups('groupId')",
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
# <a name="c"></a>[<span data-ttu-id="7a977-185">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-188">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a977-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-189">Response</span></span>
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

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="7a977-190">Exemplo 6: Criar uma equipe com um tipo de modelo de base não padrão</span><span class="sxs-lookup"><span data-stu-id="7a977-190">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="7a977-191">Os tipos de modelos base são modelos especiais criados pela Microsoft para setores específicos.</span><span class="sxs-lookup"><span data-stu-id="7a977-191">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="7a977-192">Estes modelos base geralmente contêm aplicativos proprietários que não estão disponíveis nas lojas, e propriedade de equipe que ainda não tem suporte individual nos modelos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7a977-192">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="7a977-193">Para criar uma equipe a partir de um modelo base não padrão, você vai precisar alterar a propriedade `template@odata.bind` no corpo da solicitação de `standard` para indicar o que você deseja criar para o modelo base padrão.</span><span class="sxs-lookup"><span data-stu-id="7a977-193">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="7a977-194">Para saber mais sobre tipos de modelos base com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="7a977-194">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-195">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a977-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-196">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7a977-197">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-200">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a977-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-201">Response</span></span>
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

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="7a977-202">Exemplo 7: Criar uma equipe com um tipo de modelo base não padrão com propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="7a977-202">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="7a977-203">Os tipos de modelos base podem ser estendidos com propriedade adicionais, permitindo que você crie sobre um modelo base existente com configurações, canais, aplicativos ou guias de equipe adicionais.</span><span class="sxs-lookup"><span data-stu-id="7a977-203">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="7a977-204">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="7a977-204">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-205">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a977-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a977-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
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
# <a name="c"></a>[<span data-ttu-id="7a977-207">C#</span><span class="sxs-lookup"><span data-stu-id="7a977-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a977-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a977-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a977-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a977-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a977-210">Java</span><span class="sxs-lookup"><span data-stu-id="7a977-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a977-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-211">Response</span></span>
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

### <a name="example-8-create-a-team-in-migration-mode"></a><span data-ttu-id="7a977-212">Exemplo 8: Criar uma equipe no modo de migração</span><span class="sxs-lookup"><span data-stu-id="7a977-212">Example 8: Create a team in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="7a977-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a977-213">Request</span></span>

<span data-ttu-id="7a977-214">O exemplo a seguir mostra como criar uma equipe para mensagens importadas.</span><span class="sxs-lookup"><span data-stu-id="7a977-214">The following example shows how to create a team for imported messages.</span></span>

><span data-ttu-id="7a977-215">**Observação:** No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="7a977-215">**Note:** In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.|</span></span>

><span data-ttu-id="7a977-216">**Observação:** Equipes criadas no modo de migração só suportam o modelo `standard`.</span><span class="sxs-lookup"><span data-stu-id="7a977-216">**Note:** Teams created in migration mode only support the `standard` template.</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "@microsoft.graph.teamCreationMode": "migration",
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="7a977-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a977-217">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
```

#### <a name="error-response"></a><span data-ttu-id="7a977-218">Resposta de erro</span><span class="sxs-lookup"><span data-stu-id="7a977-218">Error response</span></span>

<span data-ttu-id="7a977-219">Se a solicitação não for bem-sucedida, este método retorna um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="7a977-219">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> 

```http
400 Bad Request
```

<span data-ttu-id="7a977-220">Os seguintes são motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="7a977-220">The following are common reasons for this response:</span></span>

* <span data-ttu-id="7a977-221">**createdDateTime** é definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="7a977-221">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="7a977-222">**createdDateTime** está especificado corretamente, mas o atributo da instância **teamCreationMode** está ausente ou definido com um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="7a977-222">**createdDateTime** is correctly specified but the **teamCreationMode** instance attribute is missing or set to an invalid value.</span></span>


## <a name="see-also"></a><span data-ttu-id="7a977-223">Confira também</span><span class="sxs-lookup"><span data-stu-id="7a977-223">See also</span></span>

* [<span data-ttu-id="7a977-224">Migração completa para uma equipe</span><span class="sxs-lookup"><span data-stu-id="7a977-224">Complete migration for a team</span></span>](team-completemigration.md)
* [<span data-ttu-id="7a977-225">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7a977-225">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="7a977-226">Create channel</span><span class="sxs-lookup"><span data-stu-id="7a977-226">Create channel</span></span>](channel-post.md)
* [<span data-ttu-id="7a977-227">Modelos disponíveis</span><span class="sxs-lookup"><span data-stu-id="7a977-227">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
* [<span data-ttu-id="7a977-228">Introdução aos modelos de Equipes de varejo</span><span class="sxs-lookup"><span data-stu-id="7a977-228">Getting started with Retail Teams templates</span></span>](/MicrosoftTeams/get-started-with-retail-teams-templates)
* [<span data-ttu-id="7a977-229">Introdução aos modelos de Equipes médicas</span><span class="sxs-lookup"><span data-stu-id="7a977-229">Getting started with Healthcare Teams templates</span></span>](/MicrosoftTeams/healthcare/healthcare-templates)
* [<span data-ttu-id="7a977-230">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="7a977-230">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
