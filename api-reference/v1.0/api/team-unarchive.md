---
title: Desarquivar equipe
description: Restaurar uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe. As equipes são arquivadas usando a API de arquivo morto.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 011b68f2e85c041ccb0f654295dfaf1a42d5d237
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024221"
---
# <a name="unarchive-team"></a><span data-ttu-id="3eae7-105">Desarquivar equipe</span><span class="sxs-lookup"><span data-stu-id="3eae7-105">Unarchive team</span></span>



<span data-ttu-id="3eae7-106">Restaurar uma [equipe](../resources/team.md)arquivada.</span><span class="sxs-lookup"><span data-stu-id="3eae7-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="3eae7-107">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe.</span><span class="sxs-lookup"><span data-stu-id="3eae7-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="3eae7-108">As equipes são arquivadas usando a API de [arquivo morto](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="3eae7-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="3eae7-109">O desarquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="3eae7-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="3eae7-110">Uma equipe é desarquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="3eae7-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eae7-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3eae7-111">Permissions</span></span>
<span data-ttu-id="3eae7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eae7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eae7-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eae7-114">Permission type</span></span>      | <span data-ttu-id="3eae7-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3eae7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eae7-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eae7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3eae7-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eae7-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3eae7-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eae7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eae7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eae7-119">Not supported.</span></span>    |
|<span data-ttu-id="3eae7-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eae7-120">Application</span></span> | <span data-ttu-id="3eae7-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eae7-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="3eae7-122">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3eae7-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3eae7-123">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="3eae7-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3eae7-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eae7-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="3eae7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eae7-125">Request headers</span></span>
| <span data-ttu-id="3eae7-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3eae7-126">Header</span></span>       | <span data-ttu-id="3eae7-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3eae7-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3eae7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eae7-128">Authorization</span></span>  | <span data-ttu-id="3eae7-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eae7-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3eae7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eae7-131">Request body</span></span>
<span data-ttu-id="3eae7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3eae7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eae7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eae7-133">Response</span></span>

<span data-ttu-id="3eae7-134">Se o desarquivamento for iniciado com êxito, este método retornará `202 Accepted` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="3eae7-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="3eae7-135">A resposta também conterá um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para lidar com o cancelamento de arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="3eae7-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="3eae7-136">Verifique o status da operação de desarquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="3eae7-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="3eae7-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eae7-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3eae7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eae7-138">Request</span></span>
<span data-ttu-id="3eae7-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eae7-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="3eae7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eae7-140">Response</span></span>
<span data-ttu-id="3eae7-141">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3eae7-141">The following is an example of a response.</span></span>
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
