---
title: Criar canal
description: Crie um novo canal em uma equipe, conforme especificado no corpo da solicitação.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7ab9a2d0bdd204e77b9bc149860e9fdfab9d2fcf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202692"
---
# <a name="create-channel"></a><span data-ttu-id="5ec99-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="5ec99-103">Create channel</span></span>

<span data-ttu-id="5ec99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ec99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ec99-105">Crie um novo [canal](../resources/channel.md) em uma equipe, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ec99-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ec99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ec99-106">Permissions</span></span>

<span data-ttu-id="5ec99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ec99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ec99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ec99-109">Permission type</span></span>      | <span data-ttu-id="5ec99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ec99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ec99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ec99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ec99-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec99-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="5ec99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ec99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ec99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ec99-114">Not supported.</span></span>    |
|<span data-ttu-id="5ec99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ec99-115">Application</span></span> | <span data-ttu-id="5ec99-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec99-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="5ec99-117">**Observações**: Permissões marcadas com \* use [o consentimento específico do recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="5ec99-117">**Notes**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>
>
> <span data-ttu-id="5ec99-118">Esta API dá suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5ec99-118">This API supports admin permissions.</span></span> <span data-ttu-id="5ec99-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="5ec99-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>
>
> <span data-ttu-id="5ec99-120">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados usando APIs de trabalho em equipe.Migrate.All e/ou [migração.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="5ec99-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="5ec99-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ec99-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="5ec99-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec99-122">Request headers</span></span>

| <span data-ttu-id="5ec99-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ec99-123">Header</span></span>       | <span data-ttu-id="5ec99-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5ec99-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ec99-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ec99-125">Authorization</span></span>  | <span data-ttu-id="5ec99-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ec99-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ec99-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ec99-128">Content-Type</span></span>  | <span data-ttu-id="5ec99-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ec99-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ec99-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec99-131">Request body</span></span>

<span data-ttu-id="5ec99-132">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5ec99-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5ec99-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec99-133">Response</span></span>

<span data-ttu-id="5ec99-134">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec99-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ec99-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ec99-135">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="5ec99-136">Exemplo 1: Criar um canal padrão</span><span class="sxs-lookup"><span data-stu-id="5ec99-136">Example 1: Create a standard channel</span></span>
#### <a name="request"></a><span data-ttu-id="5ec99-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec99-137">Request</span></span>

<span data-ttu-id="5ec99-138">O exemplo a seguir mostra uma solicitação para criar um canal padrão.</span><span class="sxs-lookup"><span data-stu-id="5ec99-138">The following example shows a request to create a standard channel.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```


#### <a name="response"></a><span data-ttu-id="5ec99-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec99-139">Response</span></span>

<span data-ttu-id="5ec99-140">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec99-140">The following example shows the response.</span></span>

> <span data-ttu-id="5ec99-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ec99-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="5ec99-142">Exemplo 2: Criar canal privado em nome do usuário</span><span class="sxs-lookup"><span data-stu-id="5ec99-142">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="5ec99-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec99-143">Request</span></span>

<span data-ttu-id="5ec99-144">O exemplo a seguir mostra uma solicitação para criar um canal privado e adicionar um usuário como proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="5ec99-144">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Graph.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')",
           "roles":["owner"]
        }
     ]
}
```



#### <a name="response"></a><span data-ttu-id="5ec99-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec99-145">Response</span></span>

<span data-ttu-id="5ec99-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec99-146">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:33b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="5ec99-147">Exemplo 3: Criar um canal no modo de migração</span><span class="sxs-lookup"><span data-stu-id="5ec99-147">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="5ec99-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec99-148">Request</span></span>

<span data-ttu-id="5ec99-149">O exemplo a seguir mostra como criar um canal que será usado para importar mensagens.</span><span class="sxs-lookup"><span data-stu-id="5ec99-149">The following example shows how to create a channel that will be used for importing messages.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Import_150958_99z",
  "description": "Import_150958_99z",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```


#### <a name="response"></a><span data-ttu-id="5ec99-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec99-150">Response</span></span>

<span data-ttu-id="5ec99-151">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec99-151">The following example shows the response.</span></span> <span data-ttu-id="5ec99-152">O header Content-Location na resposta especifica o caminho para o canal que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="5ec99-152">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="5ec99-153">Depois de provisionado, esse canal pode ser usado para [importar mensagens](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="5ec99-153">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_for_migration",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Location: /teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:987c7a9fbe6447ccb3ea31bcded5c75c@thread.tacv2",
    "createdDateTime": null,
    "displayName": "Import_150958_99z",
    "description": "Import_150958_99z",
    "isFavoriteByDefault": null,
    "email": null,
    "webUrl": null,
    "membershipType": null,
    "moderationSettings": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
