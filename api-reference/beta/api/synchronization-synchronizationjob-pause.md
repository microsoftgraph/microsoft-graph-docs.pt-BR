---
title: 'synchronizationJob: pausar'
description: Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada inicial é feita.
localization_priority: Normal
ms.openlocfilehash: 29bef888a86f1b434a347a62ffb255f90de36ca7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330513"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="a0b24-104">synchronizationJob: pausar</span><span class="sxs-lookup"><span data-stu-id="a0b24-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0b24-105">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="a0b24-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="a0b24-106">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="a0b24-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0b24-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0b24-107">Permissions</span></span>
<span data-ttu-id="a0b24-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0b24-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0b24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0b24-110">Permission type</span></span>                        | <span data-ttu-id="a0b24-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0b24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0b24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0b24-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="a0b24-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0b24-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a0b24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0b24-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a0b24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0b24-115">Not supported.</span></span>  |
|<span data-ttu-id="a0b24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0b24-116">Application</span></span>                            |<span data-ttu-id="a0b24-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0b24-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a0b24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0b24-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="a0b24-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b24-119">Request headers</span></span>

| <span data-ttu-id="a0b24-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a0b24-120">Name</span></span>           | <span data-ttu-id="a0b24-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0b24-121">Type</span></span>    | <span data-ttu-id="a0b24-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0b24-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a0b24-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0b24-123">Authorization</span></span>  | <span data-ttu-id="a0b24-124">string</span><span class="sxs-lookup"><span data-stu-id="a0b24-124">string</span></span>  | <span data-ttu-id="a0b24-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0b24-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0b24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b24-127">Request body</span></span>

<span data-ttu-id="a0b24-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0b24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0b24-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0b24-129">Response</span></span>

<span data-ttu-id="a0b24-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a0b24-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="a0b24-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0b24-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0b24-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0b24-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0b24-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b24-133">Request</span></span>
<span data-ttu-id="a0b24-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0b24-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="a0b24-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0b24-135">Response</span></span>
<span data-ttu-id="a0b24-136">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a0b24-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
