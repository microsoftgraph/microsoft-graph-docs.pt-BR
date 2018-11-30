---
title: Equipe de unarchive
description: Restaure uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe. As equipes são arquivadas usando a API de arquivamento.
ms.openlocfilehash: 4a90be4c5b2488bf72123cabe1da3aacf856e9d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004939"
---
# <a name="unarchive-team"></a><span data-ttu-id="6a08a-105">Equipe de unarchive</span><span class="sxs-lookup"><span data-stu-id="6a08a-105">Unarchive team</span></span>



<span data-ttu-id="6a08a-106">Restaure uma [equipe](../resources/team.md)de arquivados.</span><span class="sxs-lookup"><span data-stu-id="6a08a-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="6a08a-107">Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe.</span><span class="sxs-lookup"><span data-stu-id="6a08a-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="6a08a-108">As equipes são arquivadas usando o [arquivo morto](team-archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="6a08a-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="6a08a-109">Unarchiving é uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="6a08a-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="6a08a-110">Uma equipe é não arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.</span><span class="sxs-lookup"><span data-stu-id="6a08a-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a08a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="6a08a-111">Permissions</span></span>
<span data-ttu-id="6a08a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a08a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a08a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a08a-114">Permission type</span></span>      | <span data-ttu-id="6a08a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a08a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a08a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a08a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6a08a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a08a-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a08a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a08a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a08a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a08a-119">Not supported.</span></span>    |
|<span data-ttu-id="6a08a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a08a-120">Application</span></span> | <span data-ttu-id="6a08a-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a08a-121">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="6a08a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a08a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="6a08a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a08a-123">Request headers</span></span>
| <span data-ttu-id="6a08a-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a08a-124">Header</span></span>       | <span data-ttu-id="6a08a-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6a08a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a08a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a08a-126">Authorization</span></span>  | <span data-ttu-id="6a08a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a08a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a08a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a08a-129">Request body</span></span>
<span data-ttu-id="6a08a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a08a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a08a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a08a-131">Response</span></span>

<span data-ttu-id="6a08a-132">Se unarchiving for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a08a-132">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="6a08a-133">A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular unarchiving da equipe.</span><span class="sxs-lookup"><span data-stu-id="6a08a-133">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="6a08a-134">Verificar o status da operação unarchiving fazendo uma solicitação GET para este local.</span><span class="sxs-lookup"><span data-stu-id="6a08a-134">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="6a08a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a08a-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6a08a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a08a-136">Request</span></span>
<span data-ttu-id="6a08a-137">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a08a-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="6a08a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a08a-138">Response</span></span>
<span data-ttu-id="6a08a-139">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="6a08a-139">The following is an example of a response.</span></span>
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
