---
title: 'synchronizationJob: pausar'
description: Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada inicial é feita.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b49d19273da7ef832e27d643c7133132c19190f9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437553"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="ac2ef-104">synchronizationJob: pausar</span><span class="sxs-lookup"><span data-stu-id="ac2ef-104">synchronizationJob: pause</span></span>

<span data-ttu-id="ac2ef-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac2ef-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac2ef-106">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-106">Temporarily stop synchronization.</span></span> <span data-ttu-id="ac2ef-107">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-107">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac2ef-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac2ef-108">Permissions</span></span>
<span data-ttu-id="ac2ef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac2ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac2ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac2ef-111">Permission type</span></span>                        | <span data-ttu-id="ac2ef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac2ef-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac2ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac2ef-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="ac2ef-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac2ef-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ac2ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac2ef-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ac2ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-116">Not supported.</span></span>  |
|<span data-ttu-id="ac2ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac2ef-117">Application</span></span>                            |<span data-ttu-id="ac2ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ac2ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac2ef-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="ac2ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac2ef-120">Request headers</span></span>

| <span data-ttu-id="ac2ef-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ac2ef-121">Name</span></span>           | <span data-ttu-id="ac2ef-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac2ef-122">Type</span></span>    | <span data-ttu-id="ac2ef-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac2ef-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ac2ef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac2ef-124">Authorization</span></span>  | <span data-ttu-id="ac2ef-125">string</span><span class="sxs-lookup"><span data-stu-id="ac2ef-125">string</span></span>  | <span data-ttu-id="ac2ef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac2ef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac2ef-128">Request body</span></span>

<span data-ttu-id="ac2ef-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac2ef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac2ef-130">Response</span></span>

<span data-ttu-id="ac2ef-131">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ac2ef-132">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac2ef-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac2ef-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac2ef-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac2ef-134">Request</span></span>
<span data-ttu-id="ac2ef-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac2ef-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac2ef-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="c"></a>[<span data-ttu-id="ac2ef-137">C#</span><span class="sxs-lookup"><span data-stu-id="ac2ef-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac2ef-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac2ef-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac2ef-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac2ef-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac2ef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac2ef-140">Response</span></span>
<span data-ttu-id="ac2ef-141">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ac2ef-141">The following is an example of a response.</span></span>
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
  "suppressions": [
  ]
}
-->
