---
title: Desarquivar equipe
description: Restaurar uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe. As equipes são arquivadas usando a API de arquivo morto.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0c39cac6a61f09c0531f1c337ff01e1b3c077b67
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2019
ms.locfileid: "31890035"
---
# <a name="unarchive-team"></a><span data-ttu-id="726b1-105">Desarquivar equipe</span><span class="sxs-lookup"><span data-stu-id="726b1-105">Unarchive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="726b1-106">Restaurar uma [equipe](../resources/team.md)arquivada.</span><span class="sxs-lookup"><span data-stu-id="726b1-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="726b1-107">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, Abiding por definições de locatários e de equipe.</span><span class="sxs-lookup"><span data-stu-id="726b1-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="726b1-108">As equipes são arquivadas usando a API de [arquivo morto](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="726b1-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="726b1-109">O desarquivamento é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="726b1-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="726b1-110">Uma equipe é desarquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="726b1-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="726b1-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="726b1-111">Permissions</span></span>
<span data-ttu-id="726b1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="726b1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="726b1-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="726b1-114">Permission type</span></span>      | <span data-ttu-id="726b1-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="726b1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="726b1-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="726b1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="726b1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="726b1-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="726b1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="726b1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="726b1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="726b1-119">Not supported.</span></span>    |
|<span data-ttu-id="726b1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="726b1-120">Application</span></span> | <span data-ttu-id="726b1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="726b1-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="726b1-122">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="726b1-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="726b1-123">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="726b1-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="726b1-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="726b1-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="726b1-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="726b1-125">Request headers</span></span>
| <span data-ttu-id="726b1-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="726b1-126">Header</span></span>       | <span data-ttu-id="726b1-127">Valor</span><span class="sxs-lookup"><span data-stu-id="726b1-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="726b1-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="726b1-128">Authorization</span></span>  | <span data-ttu-id="726b1-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="726b1-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="726b1-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="726b1-131">Request body</span></span>
<span data-ttu-id="726b1-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="726b1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="726b1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="726b1-133">Response</span></span>

<span data-ttu-id="726b1-134">Se o desarquivamento for iniciado com êxito, este método retornará `202 Accepted` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="726b1-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="726b1-135">A resposta também conterá um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para lidar com o cancelamento de arquivamento da equipe.</span><span class="sxs-lookup"><span data-stu-id="726b1-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="726b1-136">Verifique o status da operação de desarquivamento fazendo uma solicitação GET para esse local.</span><span class="sxs-lookup"><span data-stu-id="726b1-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="726b1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="726b1-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="726b1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="726b1-138">Request</span></span>
<span data-ttu-id="726b1-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="726b1-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="726b1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="726b1-140">Response</span></span>
<span data-ttu-id="726b1-141">Veja a seguir um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="726b1-141">The following is an example of a response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/team-unarchive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
