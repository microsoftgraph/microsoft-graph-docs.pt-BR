---
title: Equipe de arquivo morto
description: 'Arquive a equipe especificada. '
ms.openlocfilehash: 80c8d372c0b70548cdd887270d387f258bb92ff6
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222398"
---
# <a name="archive-team"></a><span data-ttu-id="71abf-103">Equipe de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="71abf-103">Archive team</span></span>



<span data-ttu-id="71abf-104">Arquive a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="71abf-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="71abf-105">Quando uma equipe é arquivada, os usuários podem não mais enviar como mensagens em nenhum canal na equipe de, edite o nome da equipe, descrição ou outras configurações ou em geral, verifique a maioria das alterações para a equipe.</span><span class="sxs-lookup"><span data-stu-id="71abf-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="71abf-106">As alterações de associação para a equipe continuam a ser permitido.</span><span class="sxs-lookup"><span data-stu-id="71abf-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="71abf-107">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="71abf-107">Archiving is an async operation.</span></span> <span data-ttu-id="71abf-108">Uma equipe será arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="71abf-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="71abf-109">Para arquivar equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="71abf-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="71abf-110">Para restaurar uma equipe de seu estado arquivado, use a API para [unarchive](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="71abf-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71abf-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="71abf-111">Permissions</span></span>
<span data-ttu-id="71abf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71abf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71abf-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71abf-114">Permission type</span></span>      | <span data-ttu-id="71abf-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71abf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71abf-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71abf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="71abf-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71abf-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="71abf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71abf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71abf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71abf-119">Not supported.</span></span>    |
|<span data-ttu-id="71abf-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71abf-120">Application</span></span> | <span data-ttu-id="71abf-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71abf-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="71abf-122">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="71abf-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="71abf-123">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="71abf-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="71abf-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71abf-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="71abf-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71abf-125">Request headers</span></span>
| <span data-ttu-id="71abf-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71abf-126">Header</span></span>       | <span data-ttu-id="71abf-127">Valor</span><span class="sxs-lookup"><span data-stu-id="71abf-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71abf-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="71abf-128">Authorization</span></span>  | <span data-ttu-id="71abf-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71abf-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71abf-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71abf-131">Request body</span></span>
<span data-ttu-id="71abf-132">Na solicitação, você pode _, opcionalmente,_ inclua o `shouldSetSpoSiteReadOnlyForMembers` parâmetro em um JSON body, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="71abf-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="71abf-133">Este parâmetro opcional define se deve definir permissões para os membros da equipe como somente leitura no site do Sharepoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="71abf-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="71abf-134">Definir como false ou omitindo o corpo todo resultará nesta etapa sendo ignorada.</span><span class="sxs-lookup"><span data-stu-id="71abf-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="71abf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71abf-135">Response</span></span>

<span data-ttu-id="71abf-136">Se arquivamento for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="71abf-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="71abf-137">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="71abf-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="71abf-138">Verificar o status da operação de arquivamento, tornando uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="71abf-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="71abf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71abf-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="71abf-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71abf-140">Request</span></span>
<span data-ttu-id="71abf-141">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="71abf-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="71abf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="71abf-142">Response</span></span>
<span data-ttu-id="71abf-143">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="71abf-143">The following is an example of a response.</span></span>
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
