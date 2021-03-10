---
title: Iniciar sincronizaçãoJob
description: Inicie um trabalho de sincronização existente. Se o trabalho estiver em um estado pausado, ele continuará processamento de alterações do ponto em que foi pausado. Se o trabalho estiver em quarentena, o status de quarentena será limpo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc70f816dfc1e564d27fe5c9be60580eded415e6
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626248"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="a2ca3-105">Iniciar sincronizaçãoJob</span><span class="sxs-lookup"><span data-stu-id="a2ca3-105">Start synchronizationJob</span></span>

<span data-ttu-id="a2ca3-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ca3-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2ca3-107">Inicie um trabalho de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-107">Start an existing synchronization job.</span></span> <span data-ttu-id="a2ca3-108">Se o trabalho estiver em um estado pausado, ele continuará processamento de alterações do ponto em que foi pausado.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="a2ca3-109">Se o trabalho estiver em quarentena, o status de quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-109">If the job is in quarantine, the quarantine status will be cleared.</span></span> <span data-ttu-id="a2ca3-110">Não crie scripts para chamar o trabalho inicial continuamente enquanto ele estiver em execução porque isso pode fazer com que o serviço pare de ser executado.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-110">Do not create scripts to call the start job continuously while it's running because that can cause the service to stop running.</span></span> <span data-ttu-id="a2ca3-111">Use o trabalho inicial somente quando o trabalho estiver pausado ou em quarentena.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-111">Use the start job only when the job is currently paused or in quarantine.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a2ca3-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2ca3-112">Permissions</span></span>
<span data-ttu-id="a2ca3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2ca3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ca3-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2ca3-115">Permission type</span></span>                        | <span data-ttu-id="a2ca3-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2ca3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2ca3-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2ca3-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="a2ca3-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ca3-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a2ca3-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2ca3-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a2ca3-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-120">Not supported.</span></span> |
|<span data-ttu-id="a2ca3-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2ca3-121">Application</span></span>                            |<span data-ttu-id="a2ca3-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ca3-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a2ca3-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2ca3-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="a2ca3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2ca3-124">Request headers</span></span>

| <span data-ttu-id="a2ca3-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a2ca3-125">Name</span></span>           | <span data-ttu-id="a2ca3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2ca3-126">Type</span></span>    | <span data-ttu-id="a2ca3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ca3-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a2ca3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2ca3-128">Authorization</span></span>  | <span data-ttu-id="a2ca3-129">string</span><span class="sxs-lookup"><span data-stu-id="a2ca3-129">string</span></span>  | <span data-ttu-id="a2ca3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2ca3-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2ca3-132">Request body</span></span>

<span data-ttu-id="a2ca3-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-133">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="a2ca3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2ca3-134">Response</span></span>

<span data-ttu-id="a2ca3-135">Se tiver êxito, retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-135">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="a2ca3-136">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ca3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2ca3-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a2ca3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2ca3-138">Request</span></span>
<span data-ttu-id="a2ca3-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2ca3-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2ca3-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="a2ca3-141">C#</span><span class="sxs-lookup"><span data-stu-id="a2ca3-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2ca3-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2ca3-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2ca3-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2ca3-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2ca3-144">Java</span><span class="sxs-lookup"><span data-stu-id="a2ca3-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2ca3-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2ca3-145">Response</span></span>
<span data-ttu-id="a2ca3-146">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a2ca3-146">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


