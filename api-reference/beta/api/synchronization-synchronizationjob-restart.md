---
title: Reiniciar sincronizaçãoJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente, limpa o estado de sincronização existente e os erros anteriores.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 216da34bb6900d246f990529c88bc398cc1cdcc7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50775069"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="9cabe-104">Reiniciar sincronizaçãoJob</span><span class="sxs-lookup"><span data-stu-id="9cabe-104">Restart synchronizationJob</span></span>

<span data-ttu-id="9cabe-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cabe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cabe-106">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="9cabe-106">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="9cabe-107">Opcionalmente, limpa o estado de sincronização existente e os erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="9cabe-107">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cabe-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cabe-108">Permissions</span></span>
<span data-ttu-id="9cabe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cabe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cabe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cabe-111">Permission type</span></span>                        | <span data-ttu-id="9cabe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cabe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cabe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cabe-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="9cabe-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cabe-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9cabe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cabe-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9cabe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cabe-116">Not supported.</span></span> |
|<span data-ttu-id="9cabe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cabe-117">Application</span></span>                            |<span data-ttu-id="9cabe-118">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cabe-118">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="9cabe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cabe-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="9cabe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cabe-120">Request headers</span></span>

| <span data-ttu-id="9cabe-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9cabe-121">Name</span></span>           | <span data-ttu-id="9cabe-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cabe-122">Type</span></span>    | <span data-ttu-id="9cabe-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cabe-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9cabe-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cabe-124">Authorization</span></span>  | <span data-ttu-id="9cabe-125">string</span><span class="sxs-lookup"><span data-stu-id="9cabe-125">string</span></span>  | <span data-ttu-id="9cabe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cabe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cabe-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cabe-128">Request body</span></span>

<span data-ttu-id="9cabe-129">No corpo da solicitação, forneça um objeto JSON com o parâmetro a seguir.</span><span class="sxs-lookup"><span data-stu-id="9cabe-129">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="9cabe-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9cabe-130">Parameter</span></span>     | <span data-ttu-id="9cabe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cabe-131">Type</span></span>      | <span data-ttu-id="9cabe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cabe-132">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="9cabe-133">criteria</span><span class="sxs-lookup"><span data-stu-id="9cabe-133">criteria</span></span>       |[<span data-ttu-id="9cabe-134">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="9cabe-134">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="9cabe-135">Critérios de reinicialização</span><span class="sxs-lookup"><span data-stu-id="9cabe-135">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="9cabe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cabe-136">Response</span></span>

<span data-ttu-id="9cabe-137">Se tiver êxito, retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="9cabe-137">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="9cabe-138">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cabe-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cabe-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cabe-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9cabe-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cabe-140">Request</span></span>
<span data-ttu-id="9cabe-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cabe-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cabe-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cabe-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "Watermark, Escrows, QuarantineState"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="9cabe-143">C#</span><span class="sxs-lookup"><span data-stu-id="9cabe-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cabe-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cabe-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cabe-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cabe-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cabe-146">Java</span><span class="sxs-lookup"><span data-stu-id="9cabe-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-restart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9cabe-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cabe-147">Response</span></span>
<span data-ttu-id="9cabe-148">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="9cabe-148">The following is an example of a response.</span></span>

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
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


