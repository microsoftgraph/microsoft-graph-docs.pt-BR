---
title: 'synchronizationJob: pausar'
description: Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada inicial é feita.
localization_priority: Normal
ms.openlocfilehash: 35787ef5db419a27f4490b37682e44548bffbc83
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638043"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="757cc-104">synchronizationJob: pausar</span><span class="sxs-lookup"><span data-stu-id="757cc-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="757cc-105">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="757cc-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="757cc-106">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="757cc-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="757cc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="757cc-107">Permissions</span></span>
<span data-ttu-id="757cc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="757cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="757cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="757cc-110">Permission type</span></span>                        | <span data-ttu-id="757cc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="757cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="757cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="757cc-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="757cc-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="757cc-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="757cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="757cc-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="757cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="757cc-115">Not supported.</span></span>  |
|<span data-ttu-id="757cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="757cc-116">Application</span></span>                            |<span data-ttu-id="757cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="757cc-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="757cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="757cc-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="757cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="757cc-119">Request headers</span></span>

| <span data-ttu-id="757cc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="757cc-120">Name</span></span>           | <span data-ttu-id="757cc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="757cc-121">Type</span></span>    | <span data-ttu-id="757cc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="757cc-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="757cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="757cc-123">Authorization</span></span>  | <span data-ttu-id="757cc-124">string</span><span class="sxs-lookup"><span data-stu-id="757cc-124">string</span></span>  | <span data-ttu-id="757cc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="757cc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="757cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="757cc-127">Request body</span></span>

<span data-ttu-id="757cc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="757cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="757cc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="757cc-129">Response</span></span>

<span data-ttu-id="757cc-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="757cc-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="757cc-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="757cc-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="757cc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="757cc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="757cc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="757cc-133">Request</span></span>
<span data-ttu-id="757cc-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="757cc-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="757cc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="757cc-135">Response</span></span>
<span data-ttu-id="757cc-136">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="757cc-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="757cc-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="757cc-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="757cc-138">Basic</span><span class="sxs-lookup"><span data-stu-id="757cc-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_pause-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="757cc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="757cc-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_pause-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
