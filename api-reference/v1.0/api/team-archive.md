---
title: Equipe de arquivo morto
description: 'Arquive a equipe especificada. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 5a364fe025688bf082de187940e40acdee22d6a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882849"
---
# <a name="archive-team"></a><span data-ttu-id="c7892-103">Equipe de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="c7892-103">Archive team</span></span>



<span data-ttu-id="c7892-104">Arquive a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="c7892-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="c7892-105">Quando uma equipe é arquivada, os usuários podem não mais enviar como mensagens em nenhum canal na equipe de, edite o nome da equipe, descrição ou outras configurações ou em geral, verifique a maioria das alterações para a equipe.</span><span class="sxs-lookup"><span data-stu-id="c7892-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="c7892-106">As alterações de associação para a equipe continuam a ser permitido.</span><span class="sxs-lookup"><span data-stu-id="c7892-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="c7892-107">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="c7892-107">Archiving is an async operation.</span></span> <span data-ttu-id="c7892-108">Uma equipe será arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="c7892-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="c7892-109">Para arquivar equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="c7892-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="c7892-110">Para restaurar uma equipe de seu estado arquivado, use a API para [unarchive](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="c7892-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7892-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7892-111">Permissions</span></span>
<span data-ttu-id="c7892-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7892-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7892-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7892-114">Permission type</span></span>      | <span data-ttu-id="c7892-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7892-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7892-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7892-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c7892-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7892-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7892-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7892-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7892-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7892-119">Not supported.</span></span>    |
|<span data-ttu-id="c7892-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7892-120">Application</span></span> | <span data-ttu-id="c7892-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7892-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c7892-122">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="c7892-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c7892-123">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="c7892-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7892-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7892-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="c7892-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7892-125">Request headers</span></span>
| <span data-ttu-id="c7892-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7892-126">Header</span></span>       | <span data-ttu-id="c7892-127">Valor</span><span class="sxs-lookup"><span data-stu-id="c7892-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7892-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7892-128">Authorization</span></span>  | <span data-ttu-id="c7892-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7892-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7892-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7892-131">Request body</span></span>
<span data-ttu-id="c7892-132">Na solicitação, você pode _, opcionalmente,_ inclua o `shouldSetSpoSiteReadOnlyForMembers` parâmetro em um JSON body, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="c7892-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="c7892-133">Este parâmetro opcional define se deve definir permissões para os membros da equipe como somente leitura no site do Sharepoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="c7892-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="c7892-134">Definir como false ou omitindo o corpo todo resultará nesta etapa sendo ignorada.</span><span class="sxs-lookup"><span data-stu-id="c7892-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="c7892-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7892-135">Response</span></span>

<span data-ttu-id="c7892-136">Se arquivamento for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7892-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="c7892-137">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="c7892-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="c7892-138">Verificar o status da operação de arquivamento, tornando uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="c7892-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="c7892-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7892-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c7892-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7892-140">Request</span></span>
<span data-ttu-id="c7892-141">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7892-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="c7892-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7892-142">Response</span></span>
<span data-ttu-id="c7892-143">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c7892-143">The following is an example of a response.</span></span>
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
