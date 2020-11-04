---
title: Arquivar equipe
description: 'Arquive a equipe especificada. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 19274699297334a205ae1bf397ce3c4acb4a806b
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849183"
---
# <a name="archive-team"></a><span data-ttu-id="1193a-103">Arquivar equipe</span><span class="sxs-lookup"><span data-stu-id="1193a-103">Archive team</span></span>

<span data-ttu-id="1193a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1193a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1193a-105">Arquive a [equipe ](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="1193a-105">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="1193a-106">Quando uma equipe é arquivada, os usuários não podem mais enviar ou curtir mensagens nos canais da equipe, editar o nome, a descrição ou outras configurações da equipe ou, em geral, fazer a maioria das alterações na equipe.</span><span class="sxs-lookup"><span data-stu-id="1193a-106">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="1193a-107">As alterações de associação à equipe continuam a ser permitidas.</span><span class="sxs-lookup"><span data-stu-id="1193a-107">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="1193a-108">O arquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="1193a-108">Archiving is an async operation.</span></span> <span data-ttu-id="1193a-109">Uma equipe é arquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="1193a-109">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="1193a-110">Para arquivar uma equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.</span><span class="sxs-lookup"><span data-stu-id="1193a-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="1193a-111">Para restaurar uma equipe do estado arquivado, use a API para [desarquivar](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="1193a-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1193a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="1193a-112">Permissions</span></span>
<span data-ttu-id="1193a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1193a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1193a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1193a-115">Permission type</span></span>      | <span data-ttu-id="1193a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1193a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1193a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1193a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1193a-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1193a-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1193a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1193a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1193a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1193a-120">Not supported.</span></span>    |
|<span data-ttu-id="1193a-121">Application</span><span class="sxs-lookup"><span data-stu-id="1193a-121">Application</span></span> | <span data-ttu-id="1193a-122">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1193a-122">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1193a-123">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1193a-123">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="1193a-124">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1193a-124">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="1193a-125">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1193a-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1193a-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1193a-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="1193a-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1193a-127">Request headers</span></span>
| <span data-ttu-id="1193a-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1193a-128">Header</span></span>       | <span data-ttu-id="1193a-129">Valor</span><span class="sxs-lookup"><span data-stu-id="1193a-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1193a-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1193a-130">Authorization</span></span>  | <span data-ttu-id="1193a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1193a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1193a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1193a-133">Request body</span></span>
<span data-ttu-id="1193a-134">Na solicitação, você pode _opcionalmente_ incluir o parâmetro `shouldSetSpoSiteReadOnlyForMembers` em um corpo JSON, da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="1193a-134">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="1193a-135">Este parâmetro opcional define se as permissões dos membros da equipe devem ser definidas apenas para leitura, no site do SharePoint Online associado à equipe.</span><span class="sxs-lookup"><span data-stu-id="1193a-135">This optional parameter defines whether to set permissions for team members to read-only on the SharePoint Online site associated with the team.</span></span> <span data-ttu-id="1193a-136">Essa etapa será ignorada, caso as defina como falsas ou omita o corpo completamente.</span><span class="sxs-lookup"><span data-stu-id="1193a-136">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

>[!IMPORTANT]
><span data-ttu-id="1193a-137">Não há suporte para o parâmetro `shouldSetSpoSiteReadOnlyForMembers` no contexto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1193a-137">The `shouldSetSpoSiteReadOnlyForMembers` parameter is not supported in the application context.</span></span>

## <a name="response"></a><span data-ttu-id="1193a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1193a-138">Response</span></span>

<span data-ttu-id="1193a-139">Se o arquivamento for iniciado com êxito, esse método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="1193a-139">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="1193a-140">A resposta também conterá um cabeçalho `Location`, que contém o local da [teamsAsyncOperation](../resources/teamsasyncoperation.md) criada para lidar com o arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="1193a-140">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="1193a-141">Verifique o status da operação de arquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="1193a-141">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="1193a-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1193a-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1193a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1193a-143">Request</span></span>
<span data-ttu-id="1193a-144">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1193a-144">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1193a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1193a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
# <a name="c"></a>[<span data-ttu-id="1193a-146">C#</span><span class="sxs-lookup"><span data-stu-id="1193a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/archive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1193a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1193a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/archive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1193a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1193a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/archive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1193a-149">Java</span><span class="sxs-lookup"><span data-stu-id="1193a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/archive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1193a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1193a-150">Response</span></span>
<span data-ttu-id="1193a-151">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1193a-151">The following is an example of a response.</span></span>

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

