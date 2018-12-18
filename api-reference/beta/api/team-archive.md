---
title: Equipe de arquivo morto
description: 'Arquive a equipe especificada. '
author: nkramer
ms.openlocfilehash: 6e90b7ddaae68291a0d7e970618519ddaec660e7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332645"
---
# <a name="archive-team"></a><span data-ttu-id="d8c12-103">Equipe de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="d8c12-103">Archive team</span></span>

> <span data-ttu-id="d8c12-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8c12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8c12-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8c12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8c12-106">Arquive a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="d8c12-106">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="d8c12-107">Quando uma equipe é arquivada, os usuários podem não mais enviar como mensagens em nenhum canal na equipe de, edite o nome da equipe, descrição ou outras configurações ou em geral, verifique a maioria das alterações para a equipe.</span><span class="sxs-lookup"><span data-stu-id="d8c12-107">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="d8c12-108">As alterações de associação para a equipe continuam a ser permitido.</span><span class="sxs-lookup"><span data-stu-id="d8c12-108">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="d8c12-109">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="d8c12-109">Archiving is an async operation.</span></span> <span data-ttu-id="d8c12-110">Uma equipe será arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="d8c12-110">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="d8c12-111">Para arquivar equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="d8c12-111">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="d8c12-112">Para restaurar uma equipe de seu estado arquivado, use a API para [unarchive](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="d8c12-112">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8c12-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8c12-113">Permissions</span></span>
<span data-ttu-id="d8c12-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8c12-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8c12-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8c12-116">Permission type</span></span>      | <span data-ttu-id="d8c12-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8c12-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8c12-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8c12-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d8c12-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c12-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8c12-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8c12-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8c12-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8c12-121">Not supported.</span></span>    |
|<span data-ttu-id="d8c12-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8c12-122">Application</span></span> | <span data-ttu-id="d8c12-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8c12-123">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="d8c12-124">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d8c12-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d8c12-125">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="d8c12-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8c12-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8c12-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="d8c12-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c12-127">Request headers</span></span>
| <span data-ttu-id="d8c12-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8c12-128">Header</span></span>       | <span data-ttu-id="d8c12-129">Valor</span><span class="sxs-lookup"><span data-stu-id="d8c12-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8c12-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8c12-130">Authorization</span></span>  | <span data-ttu-id="d8c12-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8c12-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8c12-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c12-133">Request body</span></span>
<span data-ttu-id="d8c12-134">Na solicitação, você pode _, opcionalmente,_ inclua o `shouldSetSpoSiteReadOnlyForMembers` parâmetro em um JSON body, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="d8c12-134">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="d8c12-135">Este parâmetro opcional define se deve definir permissões para os membros da equipe como somente leitura no site do Sharepoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="d8c12-135">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="d8c12-136">Definir como false ou omitindo o corpo todo resultará nesta etapa sendo ignorada.</span><span class="sxs-lookup"><span data-stu-id="d8c12-136">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="d8c12-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8c12-137">Response</span></span>

<span data-ttu-id="d8c12-138">Se arquivamento for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c12-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d8c12-139">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="d8c12-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="d8c12-140">Verificar o status da operação de arquivamento, tornando uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="d8c12-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="d8c12-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8c12-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d8c12-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8c12-142">Request</span></span>
<span data-ttu-id="d8c12-143">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8c12-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="d8c12-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8c12-144">Response</span></span>
<span data-ttu-id="d8c12-145">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d8c12-145">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
