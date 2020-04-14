---
title: Reiniciar synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e os erros anteriores.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9a87f7d0e2a265a6a27f661fde188909ef38310a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437523"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="26924-104">Reiniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="26924-104">Restart synchronizationJob</span></span>

<span data-ttu-id="26924-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26924-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26924-106">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="26924-106">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="26924-107">Opcionalmente limpa o estado de sincronização existente e os erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="26924-107">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="26924-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="26924-108">Permissions</span></span>
<span data-ttu-id="26924-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26924-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26924-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26924-111">Permission type</span></span>                        | <span data-ttu-id="26924-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26924-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="26924-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26924-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="26924-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26924-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="26924-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26924-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="26924-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26924-116">Not supported.</span></span> |
|<span data-ttu-id="26924-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26924-117">Application</span></span>                            |<span data-ttu-id="26924-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26924-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="26924-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26924-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="26924-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26924-120">Request headers</span></span>

| <span data-ttu-id="26924-121">Nome</span><span class="sxs-lookup"><span data-stu-id="26924-121">Name</span></span>           | <span data-ttu-id="26924-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="26924-122">Type</span></span>    | <span data-ttu-id="26924-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="26924-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="26924-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="26924-124">Authorization</span></span>  | <span data-ttu-id="26924-125">string</span><span class="sxs-lookup"><span data-stu-id="26924-125">string</span></span>  | <span data-ttu-id="26924-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26924-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26924-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26924-128">Request body</span></span>

<span data-ttu-id="26924-129">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="26924-129">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="26924-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="26924-130">Parameter</span></span>     | <span data-ttu-id="26924-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26924-131">Type</span></span>      | <span data-ttu-id="26924-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26924-132">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="26924-133">criteria</span><span class="sxs-lookup"><span data-stu-id="26924-133">criteria</span></span>       |[<span data-ttu-id="26924-134">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="26924-134">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="26924-135">Critérios de reinício</span><span class="sxs-lookup"><span data-stu-id="26924-135">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="26924-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="26924-136">Response</span></span>

<span data-ttu-id="26924-137">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="26924-137">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="26924-138">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26924-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26924-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26924-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="26924-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26924-140">Request</span></span>
<span data-ttu-id="26924-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="26924-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26924-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="26924-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26924-143">C#</span><span class="sxs-lookup"><span data-stu-id="26924-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26924-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26924-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26924-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26924-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26924-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="26924-146">Response</span></span>
<span data-ttu-id="26924-147">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="26924-147">The following is an example of a response.</span></span>

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
