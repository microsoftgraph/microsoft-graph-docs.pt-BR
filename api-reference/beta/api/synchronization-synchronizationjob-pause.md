---
title: 'synchronizationJob: pause'
description: Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, persiste, e o trabalho continuará de onde foi deixado quando uma chamada iniciar é feita.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: eba89e688b8dc9ea02fee633ee4beeb40bb55106
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137484"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="ee0a8-104">synchronizationJob: pause</span><span class="sxs-lookup"><span data-stu-id="ee0a8-104">synchronizationJob: pause</span></span>

<span data-ttu-id="ee0a8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0a8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee0a8-106">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-106">Temporarily stop synchronization.</span></span> <span data-ttu-id="ee0a8-107">Todo o progresso, incluindo o estado do trabalho, persiste, e o trabalho continuará de onde foi deixado quando [uma](../api/synchronization-synchronizationjob-start.md) chamada iniciar é feita.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-107">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee0a8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee0a8-108">Permissions</span></span>
<span data-ttu-id="ee0a8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee0a8-111">Permission type</span></span>                        | <span data-ttu-id="ee0a8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee0a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee0a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee0a8-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="ee0a8-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0a8-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ee0a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee0a8-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ee0a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-116">Not supported.</span></span>  |
|<span data-ttu-id="ee0a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee0a8-117">Application</span></span>                            |<span data-ttu-id="ee0a8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ee0a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0a8-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="ee0a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0a8-120">Request headers</span></span>

| <span data-ttu-id="ee0a8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ee0a8-121">Name</span></span>           | <span data-ttu-id="ee0a8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee0a8-122">Type</span></span>    | <span data-ttu-id="ee0a8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee0a8-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ee0a8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee0a8-124">Authorization</span></span>  | <span data-ttu-id="ee0a8-125">string</span><span class="sxs-lookup"><span data-stu-id="ee0a8-125">string</span></span>  | <span data-ttu-id="ee0a8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee0a8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0a8-128">Request body</span></span>

<span data-ttu-id="ee0a8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee0a8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee0a8-130">Response</span></span>

<span data-ttu-id="ee0a8-131">Se tiver êxito, retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ee0a8-132">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee0a8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee0a8-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee0a8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0a8-134">Request</span></span>
<span data-ttu-id="ee0a8-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee0a8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0a8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="c"></a>[<span data-ttu-id="ee0a8-137">C#</span><span class="sxs-lookup"><span data-stu-id="ee0a8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee0a8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee0a8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee0a8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee0a8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee0a8-140">Java</span><span class="sxs-lookup"><span data-stu-id="ee0a8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee0a8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee0a8-141">Response</span></span>
<span data-ttu-id="ee0a8-142">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ee0a8-142">The following is an example of a response.</span></span>
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


