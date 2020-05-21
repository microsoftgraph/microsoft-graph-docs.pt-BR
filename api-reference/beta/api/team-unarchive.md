---
title: Desarquivar equipe
description: Restaurar uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe. As equipes são arquivadas usando a API de arquivo morto.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 629b0ce0ae30956af4ebf7e38577cbfa6c3a8eb5
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335205"
---
# <a name="unarchive-team"></a><span data-ttu-id="de6df-105">Desarquivar equipe</span><span class="sxs-lookup"><span data-stu-id="de6df-105">Unarchive team</span></span>

<span data-ttu-id="de6df-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de6df-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6df-107">Restaurar uma [equipe](../resources/team.md)arquivada.</span><span class="sxs-lookup"><span data-stu-id="de6df-107">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="de6df-108">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe.</span><span class="sxs-lookup"><span data-stu-id="de6df-108">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="de6df-109">As equipes são arquivadas usando a API de [arquivo morto](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="de6df-109">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="de6df-110">O desarquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="de6df-110">Unarchiving is an async operation.</span></span> <span data-ttu-id="de6df-111">Uma equipe é desarquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="de6df-111">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="de6df-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="de6df-112">Permissions</span></span>
<span data-ttu-id="de6df-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6df-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6df-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de6df-115">Permission type</span></span>      | <span data-ttu-id="de6df-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de6df-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6df-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de6df-117">Delegated (work or school account)</span></span> | <span data-ttu-id="de6df-118">TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="de6df-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="de6df-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de6df-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6df-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de6df-120">Not supported.</span></span>    |
|<span data-ttu-id="de6df-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de6df-121">Application</span></span> | <span data-ttu-id="de6df-122">TeamSettings. Edit. Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="de6df-122">TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="de6df-123">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="de6df-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="de6df-124">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="de6df-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="de6df-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de6df-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="de6df-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de6df-126">Request headers</span></span>
| <span data-ttu-id="de6df-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de6df-127">Header</span></span>       | <span data-ttu-id="de6df-128">Valor</span><span class="sxs-lookup"><span data-stu-id="de6df-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de6df-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="de6df-129">Authorization</span></span>  | <span data-ttu-id="de6df-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6df-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de6df-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de6df-132">Request body</span></span>
<span data-ttu-id="de6df-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de6df-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de6df-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="de6df-134">Response</span></span>

<span data-ttu-id="de6df-135">Se o desarquivamento for iniciado com êxito, este método retornará um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="de6df-135">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="de6df-136">A resposta também conterá um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para lidar com o cancelamento de arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="de6df-136">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="de6df-137">Verifique o status da operação de desarquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="de6df-137">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="de6df-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de6df-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="de6df-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de6df-139">Request</span></span>
<span data-ttu-id="de6df-140">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="de6df-140">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de6df-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="de6df-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```
# <a name="c"></a>[<span data-ttu-id="de6df-142">C#</span><span class="sxs-lookup"><span data-stu-id="de6df-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unarchive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de6df-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de6df-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unarchive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de6df-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de6df-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unarchive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="de6df-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="de6df-145">Response</span></span>
<span data-ttu-id="de6df-146">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="de6df-146">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
