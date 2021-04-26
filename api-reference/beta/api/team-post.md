---
title: Criar equipe
description: Criar uma nova equipe.
author: anandjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0193d0b6e9b3c002762f13b27b2c6839ca2f7d0
ms.sourcegitcommit: 92f545d2d9af13ac7aff9932eb265f136d089f79
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51996140"
---
# <a name="create-team"></a><span data-ttu-id="1dd36-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="1dd36-103">Create team</span></span>

<span data-ttu-id="1dd36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd36-105">Criar uma nova [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1dd36-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd36-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dd36-106">Permissions</span></span>

<span data-ttu-id="1dd36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dd36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dd36-109">Permission type</span></span>                        | <span data-ttu-id="1dd36-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dd36-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1dd36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dd36-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dd36-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd36-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="1dd36-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dd36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd36-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dd36-114">Not supported.</span></span>                              |
| <span data-ttu-id="1dd36-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dd36-115">Application</span></span>                            | <span data-ttu-id="1dd36-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd36-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1dd36-117">**Observação**: A permissão Teamwork.Migrate.All é *somente* suportado para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="1dd36-117">**Note**: The Teamwork.Migrate.All permission is *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="1dd36-118">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="1dd36-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="1dd36-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="1dd36-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-120">Request headers</span></span>

| <span data-ttu-id="1dd36-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dd36-121">Header</span></span>        | <span data-ttu-id="1dd36-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1dd36-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1dd36-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dd36-123">Authorization</span></span> | <span data-ttu-id="1dd36-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dd36-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dd36-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1dd36-126">Content-Type</span></span>  | <span data-ttu-id="1dd36-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dd36-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dd36-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-129">Request body</span></span>

<span data-ttu-id="1dd36-130">No corpo da solicitação, forneça uma representação JSON de um objeto [team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1dd36-130">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1dd36-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-131">Response</span></span>

<span data-ttu-id="1dd36-132">Se bem-sucedida, essa API retornará uma resposta `202 Accepted` contendo um link para a [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="1dd36-132">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="1dd36-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1dd36-133">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="1dd36-134">Exemplo 1: Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="1dd36-134">Example 1: Delegated permissions</span></span>

<span data-ttu-id="1dd36-135">Este é um exemplo de uma solicitação mínima.</span><span class="sxs-lookup"><span data-stu-id="1dd36-135">The following is an example of a minimal request.</span></span> <span data-ttu-id="1dd36-136">Ao omitir outras propriedades, o cliente está, implicitamente, obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="1dd36-136">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd36-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1dd36-139">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-142">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->

##### <a name="response"></a><span data-ttu-id="1dd36-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-143">Response</span></span>

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

### <a name="example-2-application-permissions"></a><span data-ttu-id="1dd36-144">Exemplo 2: Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1dd36-144">Example 2: Application permissions</span></span>

<span data-ttu-id="1dd36-145">Aqui está um exemplo de uma solicitação mínima usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dd36-145">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="1dd36-146">Ao omitir outras propriedades, o cliente está implicitamente obtendo padrões do modelo predefinido representado por `template`.</span><span class="sxs-lookup"><span data-stu-id="1dd36-146">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="1dd36-147">Ao emitir uma solicitação com permissões de aplicativo, um [usuário](../resources/user.md) deve ser especificado no conjunto `members`.</span><span class="sxs-lookup"><span data-stu-id="1dd36-147">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `members` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-148">Request</span></span>
<!-- markdownlint-disable MD025 -->

# <a name="http"></a>[<span data-ttu-id="1dd36-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-149">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="1dd36-150">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-153">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1dd36-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-154">Response</span></span>
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

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="1dd36-155">Exemplo 3: Criar uma equipe com vários canais, aplicativos instalados e guias fixadas usando permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="1dd36-155">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="1dd36-156">Aqui está uma solicitação com um conteúdo completo.</span><span class="sxs-lookup"><span data-stu-id="1dd36-156">The following is a request with a full payload.</span></span> <span data-ttu-id="1dd36-157">O cliente pode substituir os valores no modelo-base e adicionar itens com valor de matriz na máxima extensão permitida por regras de validação para a `specialization`.</span><span class="sxs-lookup"><span data-stu-id="1dd36-157">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-158">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd36-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1dd36-160">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-full-payload-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-full-payload-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-full-payload-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-163">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-post-full-payload-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1dd36-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-164">Response</span></span>
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

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="1dd36-165">Exemplo 4: criar uma equipe a partir do grupo</span><span class="sxs-lookup"><span data-stu-id="1dd36-165">Example 4: Create a team from group</span></span>

<span data-ttu-id="1dd36-166">O exemplo a seguir mostra como você pode criar uma nova [equipe](../resources/team.md) a partir de um [grupo](../resources/group.md), dado um **groupId**.</span><span class="sxs-lookup"><span data-stu-id="1dd36-166">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="1dd36-167">Observações sobre essa chamada:</span><span class="sxs-lookup"><span data-stu-id="1dd36-167">A few things to note about this call:</span></span>

* <span data-ttu-id="1dd36-168">Para criar uma equipe, o grupo a partir do qual você a está criando deve ter pelo menos um proprietário.</span><span class="sxs-lookup"><span data-stu-id="1dd36-168">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="1dd36-169">A equipe criada será sempre herdeira do nome de exibição, visibilidade, especialização e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="1dd36-169">The team that's created will always inherit from the group's display name, visibility, specialization, and members.</span></span> <span data-ttu-id="1dd36-170">Portanto, ao tomar essa decisão com a propriedade **group@odata.bind**, a inclusão da equipe **displayName**, **visibilidade**, **especialização** ou propriedades **owners@odata.bind** retornarão um erro.</span><span class="sxs-lookup"><span data-stu-id="1dd36-170">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **members@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="1dd36-171">Se o grupo foi criado há menos de 15 minutos, é possível que a chamada Criar equipe falhe com um código de erro 404 devido a atrasos na replicação.</span><span class="sxs-lookup"><span data-stu-id="1dd36-171">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="1dd36-172">Recomendamos que você repita a chamada Criar equipe três vezes, com um atraso de 10 segundos entre as chamadas.</span><span class="sxs-lookup"><span data-stu-id="1dd36-172">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd36-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/beta/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
}
```

# <a name="c"></a>[<span data-ttu-id="1dd36-175">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-178">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1dd36-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-179">Response</span></span>
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

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="1dd36-180">Exemplo 5: Criar uma equipe a partir de um grupo com vários canais, aplicativos instalados e guias fixadas</span><span class="sxs-lookup"><span data-stu-id="1dd36-180">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="1dd36-181">A seguir está uma solicitação que converte um grupo existente com propriedades estendidas que criarão a equipe com vários canais, aplicativos instalados e guias fixadas.</span><span class="sxs-lookup"><span data-stu-id="1dd36-181">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="1dd36-182">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="1dd36-182">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-183">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd36-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/beta/teamsTemplates('standard')",
   "group@odata.bind":"https://graph.microsoft.com/beta/groups('dbd8de4f-5d47-48da-87f1-594bed003375')",
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
# <a name="c"></a>[<span data-ttu-id="1dd36-185">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-188">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1dd36-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-189">Response</span></span>
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

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="1dd36-190">Exemplo 6: Criar uma equipe com um tipo de modelo de base não padrão</span><span class="sxs-lookup"><span data-stu-id="1dd36-190">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="1dd36-191">Os tipos de modelos base são modelos especiais criados pela Microsoft para setores específicos.</span><span class="sxs-lookup"><span data-stu-id="1dd36-191">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="1dd36-192">Estes modelos base geralmente contêm aplicativos proprietários que não estão disponíveis nas lojas, e propriedade de equipe que ainda não tem suporte individual nos modelos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1dd36-192">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="1dd36-193">Para criar uma equipe a partir de um modelo base não padrão, você vai precisar alterar a propriedade `template@odata.bind` no corpo da solicitação de `standard` para indicar o que você deseja criar para o modelo base padrão.</span><span class="sxs-lookup"><span data-stu-id="1dd36-193">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="1dd36-194">Para saber mais sobre tipos de modelos base com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="1dd36-194">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-195">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd36-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-196">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1dd36-197">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-200">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1dd36-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-201">Response</span></span>
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

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="1dd36-202">Exemplo 7: Criar uma equipe com um tipo de modelo base não padrão com propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="1dd36-202">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="1dd36-203">Os tipos de modelos base podem ser estendidos com propriedade adicionais, permitindo que você crie sobre um modelo base existente com configurações, canais, aplicativos ou guias de equipe adicionais.</span><span class="sxs-lookup"><span data-stu-id="1dd36-203">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="1dd36-204">Para saber mais sobre os tipos de modelos base com suporte e propriedades com suporte, confira [Comece a trabalhar com modelos do Teams](/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="1dd36-204">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-205">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd36-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd36-206">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1dd36-207">C#</span><span class="sxs-lookup"><span data-stu-id="1dd36-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd36-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd36-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd36-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd36-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd36-210">Java</span><span class="sxs-lookup"><span data-stu-id="1dd36-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-team-from-non-standard2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1dd36-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-211">Response</span></span>
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

### <a name="example-8-create-a-team-in-migration-mode"></a><span data-ttu-id="1dd36-212">Exemplo 8: Criar uma equipe no modo de migração</span><span class="sxs-lookup"><span data-stu-id="1dd36-212">Example 8: Create a team in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd36-213">Request</span></span>

<span data-ttu-id="1dd36-214">O exemplo a seguir mostra como criar uma equipe para mensagens importadas.</span><span class="sxs-lookup"><span data-stu-id="1dd36-214">The following example shows how to create a team for imported messages.</span></span>

><span data-ttu-id="1dd36-215">**Observação**: no futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="1dd36-215">**Note:** In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

><span data-ttu-id="1dd36-216">**Observação:** Equipes criadas no modo de migração só suportam o modelo `standard`.</span><span class="sxs-lookup"><span data-stu-id="1dd36-216">**Note:** Teams created in migration mode only support the `standard` template.</span></span>

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

#### <a name="response"></a><span data-ttu-id="1dd36-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd36-217">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
```

#### <a name="error-response"></a><span data-ttu-id="1dd36-218">Resposta de erro</span><span class="sxs-lookup"><span data-stu-id="1dd36-218">Error response</span></span>

<span data-ttu-id="1dd36-219">Se a solicitação não for bem-sucedida, este método retorna um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="1dd36-219">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> 

```http
400 Bad Request
```

<span data-ttu-id="1dd36-220">Os seguintes são motivos comuns para esta resposta:</span><span class="sxs-lookup"><span data-stu-id="1dd36-220">The following are common reasons for this response:</span></span>

* <span data-ttu-id="1dd36-221">**createdDateTime** é definido no futuro.</span><span class="sxs-lookup"><span data-stu-id="1dd36-221">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="1dd36-222">**createdDateTime** está especificado corretamente, mas o atributo da instância **teamCreationMode** está ausente ou definido com um valor inválido.</span><span class="sxs-lookup"><span data-stu-id="1dd36-222">**createdDateTime** is correctly specified but the **teamCreationMode** instance attribute is missing or set to an invalid value.</span></span>


## <a name="see-also"></a><span data-ttu-id="1dd36-223">Confira também</span><span class="sxs-lookup"><span data-stu-id="1dd36-223">See also</span></span>

* [<span data-ttu-id="1dd36-224">Migração completa para uma equipe</span><span class="sxs-lookup"><span data-stu-id="1dd36-224">Complete migration for a team</span></span>](team-completemigration.md)
* [<span data-ttu-id="1dd36-225">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1dd36-225">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="1dd36-226">Create channel</span><span class="sxs-lookup"><span data-stu-id="1dd36-226">Create channel</span></span>](channel-post.md)
* [<span data-ttu-id="1dd36-227">Modelos disponíveis</span><span class="sxs-lookup"><span data-stu-id="1dd36-227">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
* [<span data-ttu-id="1dd36-228">Introdução aos modelos de Equipes de varejo</span><span class="sxs-lookup"><span data-stu-id="1dd36-228">Getting started with Retail Teams templates</span></span>](/MicrosoftTeams/get-started-with-retail-teams-templates)
* [<span data-ttu-id="1dd36-229">Introdução aos modelos de Equipes médicas</span><span class="sxs-lookup"><span data-stu-id="1dd36-229">Getting started with Healthcare Teams templates</span></span>](/MicrosoftTeams/healthcare/healthcare-templates)
* [<span data-ttu-id="1dd36-230">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="1dd36-230">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
