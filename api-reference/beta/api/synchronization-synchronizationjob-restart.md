---
title: Reiniciar synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e os erros anteriores.
localization_priority: Normal
ms.openlocfilehash: ae88562bba0c3d0b9d618272015f2c9044fc8c95
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638022"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="1486d-104">Reiniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1486d-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1486d-105">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="1486d-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="1486d-106">Opcionalmente limpa o estado de sincronização existente e os erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="1486d-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="1486d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1486d-107">Permissions</span></span>
<span data-ttu-id="1486d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1486d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1486d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1486d-110">Permission type</span></span>                        | <span data-ttu-id="1486d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1486d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1486d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1486d-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="1486d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1486d-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1486d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1486d-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1486d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1486d-115">Not supported.</span></span> |
|<span data-ttu-id="1486d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1486d-116">Application</span></span>                            |<span data-ttu-id="1486d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1486d-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1486d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1486d-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="1486d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1486d-119">Request headers</span></span>

| <span data-ttu-id="1486d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1486d-120">Name</span></span>           | <span data-ttu-id="1486d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1486d-121">Type</span></span>    | <span data-ttu-id="1486d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1486d-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1486d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1486d-123">Authorization</span></span>  | <span data-ttu-id="1486d-124">string</span><span class="sxs-lookup"><span data-stu-id="1486d-124">string</span></span>  | <span data-ttu-id="1486d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1486d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1486d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1486d-127">Request body</span></span>

<span data-ttu-id="1486d-128">No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1486d-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="1486d-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1486d-129">Parameter</span></span>     | <span data-ttu-id="1486d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1486d-130">Type</span></span>      | <span data-ttu-id="1486d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1486d-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1486d-132">criteria</span><span class="sxs-lookup"><span data-stu-id="1486d-132">criteria</span></span>       |[<span data-ttu-id="1486d-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="1486d-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="1486d-134">Critérios de reinício</span><span class="sxs-lookup"><span data-stu-id="1486d-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="1486d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1486d-135">Response</span></span>

<span data-ttu-id="1486d-136">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1486d-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="1486d-137">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1486d-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1486d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1486d-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1486d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1486d-139">Request</span></span>
<span data-ttu-id="1486d-140">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1486d-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1486d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1486d-141">Response</span></span>
<span data-ttu-id="1486d-142">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1486d-142">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1486d-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1486d-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1486d-144">Basic</span><span class="sxs-lookup"><span data-stu-id="1486d-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1486d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1486d-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
