---
title: Reiniciar synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e os erros anteriores.
localization_priority: Normal
ms.openlocfilehash: 2c14a77553054fe689aba90bc8eeb53854f63642
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457012"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="0517c-104">Reiniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0517c-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0517c-105">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="0517c-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="0517c-106">Opcionalmente limpa o estado de sincronização existente e os erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="0517c-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="0517c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0517c-107">Permissions</span></span>
<span data-ttu-id="0517c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0517c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0517c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0517c-110">Permission type</span></span>                        | <span data-ttu-id="0517c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0517c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0517c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0517c-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="0517c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0517c-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0517c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0517c-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0517c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0517c-115">Not supported.</span></span> |
|<span data-ttu-id="0517c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0517c-116">Application</span></span>                            |<span data-ttu-id="0517c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0517c-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="0517c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0517c-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="0517c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0517c-119">Request headers</span></span>

| <span data-ttu-id="0517c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0517c-120">Name</span></span>           | <span data-ttu-id="0517c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0517c-121">Type</span></span>    | <span data-ttu-id="0517c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0517c-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0517c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0517c-123">Authorization</span></span>  | <span data-ttu-id="0517c-124">string</span><span class="sxs-lookup"><span data-stu-id="0517c-124">string</span></span>  | <span data-ttu-id="0517c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0517c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0517c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0517c-127">Request body</span></span>

<span data-ttu-id="0517c-128">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0517c-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="0517c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0517c-129">Parameter</span></span>     | <span data-ttu-id="0517c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0517c-130">Type</span></span>      | <span data-ttu-id="0517c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0517c-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0517c-132">criteria</span><span class="sxs-lookup"><span data-stu-id="0517c-132">criteria</span></span>       |[<span data-ttu-id="0517c-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="0517c-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="0517c-134">Critérios de reinício</span><span class="sxs-lookup"><span data-stu-id="0517c-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="0517c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0517c-135">Response</span></span>

<span data-ttu-id="0517c-136">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0517c-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="0517c-137">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0517c-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0517c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0517c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0517c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0517c-139">Request</span></span>
<span data-ttu-id="0517c-140">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0517c-140">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0517c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0517c-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0517c-142">C#</span><span class="sxs-lookup"><span data-stu-id="0517c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0517c-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="0517c-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0517c-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0517c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0517c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0517c-145">Response</span></span>
<span data-ttu-id="0517c-146">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0517c-146">The following is an example of a response.</span></span>

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
