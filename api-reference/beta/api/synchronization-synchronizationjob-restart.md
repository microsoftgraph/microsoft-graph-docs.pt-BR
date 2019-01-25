---
title: Reinicie o synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e erros anteriores.
localization_priority: Normal
ms.openlocfilehash: 169f95c3662fd774207584b54fcf27fb2548c795
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526722"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="ca928-104">Reinicie o synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="ca928-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca928-105">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="ca928-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="ca928-106">Opcionalmente limpa o estado de sincronização existente e erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="ca928-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca928-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca928-107">Permissions</span></span>
<span data-ttu-id="ca928-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca928-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca928-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca928-110">Permission type</span></span>                        | <span data-ttu-id="ca928-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca928-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca928-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca928-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="ca928-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca928-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ca928-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca928-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ca928-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca928-115">Not supported.</span></span> |
|<span data-ttu-id="ca928-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca928-116">Application</span></span>                            |<span data-ttu-id="ca928-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca928-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ca928-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca928-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="ca928-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca928-119">Request headers</span></span>

| <span data-ttu-id="ca928-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ca928-120">Name</span></span>           | <span data-ttu-id="ca928-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca928-121">Type</span></span>    | <span data-ttu-id="ca928-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca928-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ca928-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca928-123">Authorization</span></span>  | <span data-ttu-id="ca928-124">string</span><span class="sxs-lookup"><span data-stu-id="ca928-124">string</span></span>  | <span data-ttu-id="ca928-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca928-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca928-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca928-127">Request body</span></span>

<span data-ttu-id="ca928-128">No corpo da solicitação, fornecem um objeto JSON com o parâmetro a seguir.</span><span class="sxs-lookup"><span data-stu-id="ca928-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="ca928-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ca928-129">Parameter</span></span>     | <span data-ttu-id="ca928-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca928-130">Type</span></span>      | <span data-ttu-id="ca928-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca928-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ca928-132">critérios</span><span class="sxs-lookup"><span data-stu-id="ca928-132">criteria</span></span>       |[<span data-ttu-id="ca928-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="ca928-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="ca928-134">Reinicie os critérios</span><span class="sxs-lookup"><span data-stu-id="ca928-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="ca928-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca928-135">Response</span></span>

<span data-ttu-id="ca928-136">Se tiver êxito, retorna um `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="ca928-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ca928-137">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca928-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca928-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca928-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ca928-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca928-139">Request</span></span>
<span data-ttu-id="ca928-140">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca928-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ca928-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca928-141">Response</span></span>
<span data-ttu-id="ca928-142">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ca928-142">The following is an example of a response.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
