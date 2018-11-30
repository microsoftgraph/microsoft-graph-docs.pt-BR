---
title: 'synchronizationJob: pause'
description: Interrompa temporariamente a sincronização. Todos o andamento, incluindo o estado do trabalho é persistente e o trabalho continuará de onde ela parou quando é feita uma chamada de iniciar.
ms.openlocfilehash: dd46f5760d7ddcfff1e254d7c000e1cd80304f07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035645"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="b72ed-104">synchronizationJob: pause</span><span class="sxs-lookup"><span data-stu-id="b72ed-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="b72ed-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b72ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b72ed-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b72ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b72ed-107">Interrompa temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="b72ed-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="b72ed-108">Todos o andamento, incluindo o estado do trabalho é persistente e o trabalho continuará de onde ela parou quando uma chamada [Iniciar](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="b72ed-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="b72ed-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b72ed-109">Permissions</span></span>
<span data-ttu-id="b72ed-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b72ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b72ed-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b72ed-112">Permission type</span></span>                        | <span data-ttu-id="b72ed-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b72ed-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b72ed-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b72ed-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="b72ed-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72ed-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b72ed-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b72ed-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b72ed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b72ed-117">Not supported.</span></span>  |
|<span data-ttu-id="b72ed-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b72ed-118">Application</span></span>                            |<span data-ttu-id="b72ed-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b72ed-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b72ed-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b72ed-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="b72ed-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b72ed-121">Request headers</span></span>

| <span data-ttu-id="b72ed-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b72ed-122">Name</span></span>           | <span data-ttu-id="b72ed-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b72ed-123">Type</span></span>    | <span data-ttu-id="b72ed-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b72ed-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b72ed-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b72ed-125">Authorization</span></span>  | <span data-ttu-id="b72ed-126">string</span><span class="sxs-lookup"><span data-stu-id="b72ed-126">string</span></span>  | <span data-ttu-id="b72ed-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b72ed-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b72ed-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b72ed-129">Request body</span></span>

<span data-ttu-id="b72ed-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b72ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b72ed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b72ed-131">Response</span></span>

<span data-ttu-id="b72ed-132">Se tiver êxito, retorna um `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="b72ed-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="b72ed-133">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b72ed-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b72ed-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b72ed-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b72ed-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b72ed-135">Request</span></span>
<span data-ttu-id="b72ed-136">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b72ed-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="b72ed-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b72ed-137">Response</span></span>
<span data-ttu-id="b72ed-138">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b72ed-138">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->