---
title: Equipe de unarchive
description: Restaure uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe. As equipes são arquivadas usando a API de arquivamento.
localization_priority: Normal
ms.openlocfilehash: 512d2e69434430a19af8489082789c671efe2b7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870291"
---
# <a name="unarchive-team"></a><span data-ttu-id="75aa0-105">Equipe de unarchive</span><span class="sxs-lookup"><span data-stu-id="75aa0-105">Unarchive team</span></span>

> <span data-ttu-id="75aa0-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75aa0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75aa0-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75aa0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75aa0-108">Restaure uma [equipe](../resources/team.md)de arquivados.</span><span class="sxs-lookup"><span data-stu-id="75aa0-108">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="75aa0-109">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe.</span><span class="sxs-lookup"><span data-stu-id="75aa0-109">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="75aa0-110">As equipes são arquivadas usando o [arquivo morto](team-archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="75aa0-110">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="75aa0-111">Unarchiving é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="75aa0-111">Unarchiving is an async operation.</span></span> <span data-ttu-id="75aa0-112">Uma equipe é não arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="75aa0-112">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="75aa0-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="75aa0-113">Permissions</span></span>
<span data-ttu-id="75aa0-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75aa0-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75aa0-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75aa0-116">Permission type</span></span>      | <span data-ttu-id="75aa0-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75aa0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75aa0-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75aa0-118">Delegated (work or school account)</span></span> | <span data-ttu-id="75aa0-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75aa0-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75aa0-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75aa0-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75aa0-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75aa0-121">Not supported.</span></span>    |
|<span data-ttu-id="75aa0-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75aa0-122">Application</span></span> | <span data-ttu-id="75aa0-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75aa0-123">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="75aa0-124">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="75aa0-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="75aa0-125">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="75aa0-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="75aa0-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75aa0-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="75aa0-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75aa0-127">Request headers</span></span>
| <span data-ttu-id="75aa0-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75aa0-128">Header</span></span>       | <span data-ttu-id="75aa0-129">Valor</span><span class="sxs-lookup"><span data-stu-id="75aa0-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75aa0-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="75aa0-130">Authorization</span></span>  | <span data-ttu-id="75aa0-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75aa0-p107">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75aa0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75aa0-133">Request body</span></span>
<span data-ttu-id="75aa0-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75aa0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75aa0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="75aa0-135">Response</span></span>

<span data-ttu-id="75aa0-136">Se unarchiving for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="75aa0-136">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="75aa0-137">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular unarchiving da equipe.</span><span class="sxs-lookup"><span data-stu-id="75aa0-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="75aa0-138">Verificar o status da operação unarchiving fazendo uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="75aa0-138">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="75aa0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75aa0-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="75aa0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75aa0-140">Request</span></span>
<span data-ttu-id="75aa0-141">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="75aa0-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="75aa0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="75aa0-142">Response</span></span>
<span data-ttu-id="75aa0-143">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="75aa0-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
