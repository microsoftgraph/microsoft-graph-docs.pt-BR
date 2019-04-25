---
title: Arquivar equipe
description: 'Arquive a equipe especificada. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 28c1ea9d96d55587f95af85c9aba50a43fe08d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520246"
---
# <a name="archive-team"></a><span data-ttu-id="a0a28-103">Arquivar equipe</span><span class="sxs-lookup"><span data-stu-id="a0a28-103">Archive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0a28-104">Arquive a [equipe ](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="a0a28-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="a0a28-105">Quando uma equipe é arquivada, os usuários não podem mais enviar ou curtir mensagens nos canais da equipe, editar o nome, a descrição ou outras configurações da equipe ou, em geral, fazer a maioria das alterações na equipe.</span><span class="sxs-lookup"><span data-stu-id="a0a28-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="a0a28-106">As alterações de associação à equipe continuam a ser permitidas.</span><span class="sxs-lookup"><span data-stu-id="a0a28-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="a0a28-107">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="a0a28-107">Archiving is an async operation.</span></span> <span data-ttu-id="a0a28-108">Uma equipe é arquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="a0a28-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="a0a28-109">Para arquivar uma equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="a0a28-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="a0a28-110">Para restaurar uma equipe do estado arquivado, use a API para [desarquivar](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="a0a28-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0a28-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0a28-111">Permissions</span></span>
<span data-ttu-id="a0a28-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0a28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a28-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0a28-114">Permission type</span></span>      | <span data-ttu-id="a0a28-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0a28-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0a28-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0a28-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a0a28-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a28-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0a28-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0a28-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0a28-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0a28-119">Not supported.</span></span>    |
|<span data-ttu-id="a0a28-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0a28-120">Application</span></span> | <span data-ttu-id="a0a28-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a28-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a0a28-122">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a0a28-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a0a28-123">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a0a28-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0a28-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0a28-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="a0a28-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a28-125">Request headers</span></span>
| <span data-ttu-id="a0a28-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0a28-126">Header</span></span>       | <span data-ttu-id="a0a28-127">Valor</span><span class="sxs-lookup"><span data-stu-id="a0a28-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0a28-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0a28-128">Authorization</span></span>  | <span data-ttu-id="a0a28-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0a28-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0a28-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a28-131">Request body</span></span>
<span data-ttu-id="a0a28-132">Na solicitação, você pode _opcionalmente_ incluir o parâmetro `shouldSetSpoSiteReadOnlyForMembers` em um corpo JSON, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="a0a28-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="a0a28-133">Esse parâmetro opcional define se é necessário definir permissões para membros da equipe como somente leitura no site do SharePoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="a0a28-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="a0a28-134">Essa etapa será ignorada, caso as defina como falsas ou omita o corpo completamente.</span><span class="sxs-lookup"><span data-stu-id="a0a28-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="a0a28-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a28-135">Response</span></span>

<span data-ttu-id="a0a28-136">Se o arquivamento for iniciado com êxito, esse método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="a0a28-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="a0a28-137">A resposta também conterá um cabeçalho `Location`, que contém o local da [teamsAsyncOperation](../resources/teamsasyncoperation.md) criada para lidar com o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="a0a28-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="a0a28-138">Verifique o status da operação de arquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="a0a28-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="a0a28-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0a28-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0a28-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a28-140">Request</span></span>
<span data-ttu-id="a0a28-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0a28-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="a0a28-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a28-142">Response</span></span>
<span data-ttu-id="a0a28-143">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a0a28-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
