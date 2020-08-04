---
title: Arquivar equipe
description: 'Arquive a equipe especificada. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0a82aadc98bee975b77b5fc989361750afe3b5ec
ms.sourcegitcommit: ff3fd4ead2b864ce6abb79915a0488d0562347f8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46524323"
---
# <a name="archive-team"></a><span data-ttu-id="ae6c4-103">Arquivar equipe</span><span class="sxs-lookup"><span data-stu-id="ae6c4-103">Archive team</span></span>

<span data-ttu-id="ae6c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae6c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae6c4-105">Arquive a [equipe ](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-105">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="ae6c4-106">Quando uma equipe é arquivada, os usuários não podem mais enviar ou curtir mensagens nos canais da equipe, editar o nome, a descrição ou outras configurações da equipe ou, em geral, fazer a maioria das alterações na equipe.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-106">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="ae6c4-107">As alterações de associação à equipe continuam a ser permitidas.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-107">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="ae6c4-108">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-108">Archiving is an async operation.</span></span> <span data-ttu-id="ae6c4-109">Uma equipe é arquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-109">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="ae6c4-110">Para arquivar uma equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="ae6c4-111">Para restaurar uma equipe do estado arquivado, use a API para [desarquivar](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="ae6c4-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae6c4-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae6c4-112">Permissions</span></span>
<span data-ttu-id="ae6c4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae6c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6c4-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae6c4-115">Permission type</span></span>      | <span data-ttu-id="ae6c4-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae6c4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae6c4-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae6c4-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ae6c4-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6c4-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ae6c4-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae6c4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae6c4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-120">Not supported.</span></span>    |
|<span data-ttu-id="ae6c4-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae6c4-121">Application</span></span> |<span data-ttu-id="ae6c4-122">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6c4-122">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ae6c4-123">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ae6c4-124">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae6c4-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae6c4-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="ae6c4-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae6c4-126">Request headers</span></span>
| <span data-ttu-id="ae6c4-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae6c4-127">Header</span></span>       | <span data-ttu-id="ae6c4-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ae6c4-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae6c4-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae6c4-129">Authorization</span></span>  | <span data-ttu-id="ae6c4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae6c4-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae6c4-132">Request body</span></span>
<span data-ttu-id="ae6c4-133">Na solicitação, você pode _opcionalmente_ incluir o parâmetro `shouldSetSpoSiteReadOnlyForMembers` em um corpo JSON, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-133">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="ae6c4-134">Este parâmetro opcional define se as permissões dos membros da equipe devem ser definidas apenas para leitura, no site do SharePoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-134">This optional parameter defines whether to set permissions for team members to read-only on the SharePoint Online site associated with the team.</span></span> <span data-ttu-id="ae6c4-135">Essa etapa será ignorada, caso as defina como falsas ou omita o corpo completamente.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-135">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

>[!IMPORTANT]
><span data-ttu-id="ae6c4-136">Não há suporte para o parâmetro `shouldSetSpoSiteReadOnlyForMembers` no contexto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-136">The `shouldSetSpoSiteReadOnlyForMembers` parameter is not supported in the application context.</span></span>

## <a name="response"></a><span data-ttu-id="ae6c4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae6c4-137">Response</span></span>

<span data-ttu-id="ae6c4-138">Se o arquivamento for iniciado com êxito, esse método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="ae6c4-139">A resposta também conterá um cabeçalho `Location`, que contém o local da [teamsAsyncOperation](../resources/teamsasyncoperation.md) criada para lidar com o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="ae6c4-140">Verifique o status da operação de arquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="ae6c4-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae6c4-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ae6c4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae6c4-142">Request</span></span>
<span data-ttu-id="ae6c4-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae6c4-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae6c4-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
# <a name="c"></a>[<span data-ttu-id="ae6c4-145">C#</span><span class="sxs-lookup"><span data-stu-id="ae6c4-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/archive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae6c4-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae6c4-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/archive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae6c4-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae6c4-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/archive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae6c4-148">Java</span><span class="sxs-lookup"><span data-stu-id="ae6c4-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/archive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ae6c4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae6c4-149">Response</span></span>
<span data-ttu-id="ae6c4-150">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ae6c4-150">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "name": "archive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
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
