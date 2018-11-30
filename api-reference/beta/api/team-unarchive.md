---
title: Equipe de unarchive
description: Restaure uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe. As equipes são arquivadas usando a API de arquivamento.
ms.openlocfilehash: 6016529f20781a66aa8c36771a56942cb471ee7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038307"
---
# <a name="unarchive-team"></a><span data-ttu-id="37dc4-105">Equipe de unarchive</span><span class="sxs-lookup"><span data-stu-id="37dc4-105">Unarchive team</span></span>

> <span data-ttu-id="37dc4-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="37dc4-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37dc4-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37dc4-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37dc4-108">Restaure uma [equipe](../resources/team.md)de arquivados.</span><span class="sxs-lookup"><span data-stu-id="37dc4-108">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="37dc4-109">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe.</span><span class="sxs-lookup"><span data-stu-id="37dc4-109">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="37dc4-110">As equipes são arquivadas usando o [arquivo morto](team-archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="37dc4-110">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="37dc4-111">Unarchiving é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="37dc4-111">Unarchiving is an async operation.</span></span> <span data-ttu-id="37dc4-112">Uma equipe é não arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="37dc4-112">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="37dc4-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="37dc4-113">Permissions</span></span>
<span data-ttu-id="37dc4-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37dc4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37dc4-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37dc4-116">Permission type</span></span>      | <span data-ttu-id="37dc4-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37dc4-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37dc4-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37dc4-118">Delegated (work or school account)</span></span> | <span data-ttu-id="37dc4-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37dc4-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="37dc4-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37dc4-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37dc4-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37dc4-121">Not supported.</span></span>    |
|<span data-ttu-id="37dc4-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37dc4-122">Application</span></span> | <span data-ttu-id="37dc4-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37dc4-123">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="37dc4-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37dc4-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="37dc4-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37dc4-125">Request headers</span></span>
| <span data-ttu-id="37dc4-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37dc4-126">Header</span></span>       | <span data-ttu-id="37dc4-127">Valor</span><span class="sxs-lookup"><span data-stu-id="37dc4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37dc4-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="37dc4-128">Authorization</span></span>  | <span data-ttu-id="37dc4-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37dc4-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37dc4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37dc4-131">Request body</span></span>
<span data-ttu-id="37dc4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37dc4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37dc4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="37dc4-133">Response</span></span>

<span data-ttu-id="37dc4-134">Se unarchiving for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="37dc4-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="37dc4-135">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular unarchiving da equipe.</span><span class="sxs-lookup"><span data-stu-id="37dc4-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="37dc4-136">Verificar o status da operação unarchiving fazendo uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="37dc4-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="37dc4-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37dc4-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="37dc4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37dc4-138">Request</span></span>
<span data-ttu-id="37dc4-139">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="37dc4-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="37dc4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="37dc4-140">Response</span></span>
<span data-ttu-id="37dc4-141">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="37dc4-141">The following is an example of a response.</span></span>
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
