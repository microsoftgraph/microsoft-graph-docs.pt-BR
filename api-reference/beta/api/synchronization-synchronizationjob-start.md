---
title: Iniciar synchronizationJob
description: Inicie um trabalho de sincronização existente. Se o trabalho estiver em um estado pausado, ele continuará processando as alterações do ponto em que foi pausado. Se o trabalho estiver em quarentena, o status da quarentena será limpo.
localization_priority: Normal
ms.openlocfilehash: 5c9e515881043ee5ceb08596f67bad4e86d34502
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638036"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="b1090-105">Iniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="b1090-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1090-106">Inicie um trabalho de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="b1090-106">Start an existing synchronization job.</span></span> <span data-ttu-id="b1090-107">Se o trabalho estiver em um estado pausado, ele continuará processando as alterações do ponto em que foi pausado.</span><span class="sxs-lookup"><span data-stu-id="b1090-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="b1090-108">Se o trabalho estiver em quarentena, o status da quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="b1090-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1090-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1090-109">Permissions</span></span>
<span data-ttu-id="b1090-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1090-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1090-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1090-112">Permission type</span></span>                        | <span data-ttu-id="b1090-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1090-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1090-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1090-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="b1090-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1090-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b1090-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1090-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b1090-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1090-117">Not supported.</span></span> |
|<span data-ttu-id="b1090-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1090-118">Application</span></span>                            |<span data-ttu-id="b1090-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1090-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1090-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1090-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="b1090-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1090-121">Request headers</span></span>

| <span data-ttu-id="b1090-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b1090-122">Name</span></span>           | <span data-ttu-id="b1090-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1090-123">Type</span></span>    | <span data-ttu-id="b1090-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1090-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b1090-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1090-125">Authorization</span></span>  | <span data-ttu-id="b1090-126">string</span><span class="sxs-lookup"><span data-stu-id="b1090-126">string</span></span>  | <span data-ttu-id="b1090-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1090-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1090-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1090-129">Request body</span></span>

<span data-ttu-id="b1090-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1090-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="b1090-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1090-131">Response</span></span>

<span data-ttu-id="b1090-132">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b1090-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="b1090-133">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1090-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1090-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1090-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1090-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1090-135">Request</span></span>
<span data-ttu-id="b1090-136">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1090-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="b1090-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1090-137">Response</span></span>
<span data-ttu-id="b1090-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b1090-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1090-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b1090-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1090-140">Basic</span><span class="sxs-lookup"><span data-stu-id="b1090-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_start-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1090-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1090-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_start-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
