---
title: Reiniciar synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e os erros anteriores.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 765b8801c808a71426fc6a5150229e028429436f
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621085"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="d41dd-104">Reiniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d41dd-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d41dd-105">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="d41dd-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="d41dd-106">Opcionalmente limpa o estado de sincronização existente e os erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="d41dd-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="d41dd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d41dd-107">Permissions</span></span>
<span data-ttu-id="d41dd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d41dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d41dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d41dd-110">Permission type</span></span>                        | <span data-ttu-id="d41dd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d41dd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d41dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d41dd-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="d41dd-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d41dd-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d41dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d41dd-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d41dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d41dd-115">Not supported.</span></span> |
|<span data-ttu-id="d41dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d41dd-116">Application</span></span>                            |<span data-ttu-id="d41dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d41dd-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="d41dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d41dd-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="d41dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d41dd-119">Request headers</span></span>

| <span data-ttu-id="d41dd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d41dd-120">Name</span></span>           | <span data-ttu-id="d41dd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d41dd-121">Type</span></span>    | <span data-ttu-id="d41dd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d41dd-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d41dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d41dd-123">Authorization</span></span>  | <span data-ttu-id="d41dd-124">string</span><span class="sxs-lookup"><span data-stu-id="d41dd-124">string</span></span>  | <span data-ttu-id="d41dd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d41dd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d41dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d41dd-127">Request body</span></span>

<span data-ttu-id="d41dd-128">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d41dd-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="d41dd-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d41dd-129">Parameter</span></span>     | <span data-ttu-id="d41dd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d41dd-130">Type</span></span>      | <span data-ttu-id="d41dd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d41dd-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d41dd-132">criteria</span><span class="sxs-lookup"><span data-stu-id="d41dd-132">criteria</span></span>       |[<span data-ttu-id="d41dd-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="d41dd-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="d41dd-134">Critérios de reinício</span><span class="sxs-lookup"><span data-stu-id="d41dd-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="d41dd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d41dd-135">Response</span></span>

<span data-ttu-id="d41dd-136">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d41dd-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="d41dd-137">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d41dd-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d41dd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d41dd-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d41dd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d41dd-139">Request</span></span>
<span data-ttu-id="d41dd-140">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d41dd-140">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d41dd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d41dd-141">HTTP</span></span>](#tab/http)
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
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d41dd-142">C#</span><span class="sxs-lookup"><span data-stu-id="d41dd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d41dd-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d41dd-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d41dd-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d41dd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d41dd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d41dd-145">Response</span></span>
<span data-ttu-id="d41dd-146">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d41dd-146">The following is an example of a response.</span></span>

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
