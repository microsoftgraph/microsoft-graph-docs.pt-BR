---
title: Desarquivar equipe
description: Restaurar uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe. As equipes são arquivadas usando a API de arquivo morto.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a6fd0aede34593d1e5ed8e0d225d16f8e74f70bf
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849162"
---
# <a name="unarchive-team"></a><span data-ttu-id="28f2f-105">Desarquivar equipe</span><span class="sxs-lookup"><span data-stu-id="28f2f-105">Unarchive team</span></span>

<span data-ttu-id="28f2f-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28f2f-106">Namespace: microsoft.graph</span></span>



<span data-ttu-id="28f2f-107">Restaurar uma [equipe](../resources/team.md)arquivada.</span><span class="sxs-lookup"><span data-stu-id="28f2f-107">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="28f2f-108">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe.</span><span class="sxs-lookup"><span data-stu-id="28f2f-108">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="28f2f-109">As equipes são arquivadas usando a API de [arquivo morto](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="28f2f-109">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="28f2f-110">O desarquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="28f2f-110">Unarchiving is an async operation.</span></span> <span data-ttu-id="28f2f-111">Uma equipe é desarquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="28f2f-111">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="28f2f-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="28f2f-112">Permissions</span></span>
<span data-ttu-id="28f2f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28f2f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28f2f-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28f2f-115">Permission type</span></span>      | <span data-ttu-id="28f2f-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28f2f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28f2f-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28f2f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="28f2f-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28f2f-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="28f2f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28f2f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28f2f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28f2f-120">Not supported.</span></span>    |
|<span data-ttu-id="28f2f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28f2f-121">Application</span></span> | <span data-ttu-id="28f2f-122">TeamSettings. ReadWrite. Group \*, TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="28f2f-122">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="28f2f-123">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="28f2f-123">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="28f2f-124">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="28f2f-124">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="28f2f-125">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="28f2f-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="28f2f-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28f2f-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="28f2f-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28f2f-127">Request headers</span></span>
| <span data-ttu-id="28f2f-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28f2f-128">Header</span></span>       | <span data-ttu-id="28f2f-129">Valor</span><span class="sxs-lookup"><span data-stu-id="28f2f-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28f2f-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="28f2f-130">Authorization</span></span>  | <span data-ttu-id="28f2f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28f2f-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28f2f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28f2f-133">Request body</span></span>
<span data-ttu-id="28f2f-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28f2f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28f2f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="28f2f-135">Response</span></span>

<span data-ttu-id="28f2f-136">Se o desarquivamento for iniciado com êxito, este método retornará um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="28f2f-136">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="28f2f-137">A resposta também conterá um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para lidar com o cancelamento de arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="28f2f-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="28f2f-138">Verifique o status da operação de desarquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="28f2f-138">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="28f2f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28f2f-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="28f2f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28f2f-140">Request</span></span>
<span data-ttu-id="28f2f-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="28f2f-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28f2f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="28f2f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```
# <a name="c"></a>[<span data-ttu-id="28f2f-143">C#</span><span class="sxs-lookup"><span data-stu-id="28f2f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unarchive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28f2f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28f2f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unarchive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28f2f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28f2f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unarchive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28f2f-146">Java</span><span class="sxs-lookup"><span data-stu-id="28f2f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unarchive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28f2f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="28f2f-147">Response</span></span>
<span data-ttu-id="28f2f-148">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="28f2f-148">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "name": "unarchive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

