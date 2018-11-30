---
title: Reinicie o synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e erros anteriores.
ms.openlocfilehash: 0b7ebfcd7b13400225d9ea149442207ecd994a8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039382"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="59f86-104">Reinicie o synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="59f86-104">Restart synchronizationJob</span></span>

> <span data-ttu-id="59f86-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="59f86-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59f86-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="59f86-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59f86-107">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="59f86-107">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="59f86-108">Opcionalmente limpa o estado de sincronização existente e erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="59f86-108">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="59f86-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="59f86-109">Permissions</span></span>
<span data-ttu-id="59f86-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59f86-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59f86-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59f86-112">Permission type</span></span>                        | <span data-ttu-id="59f86-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59f86-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="59f86-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59f86-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="59f86-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f86-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="59f86-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59f86-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="59f86-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59f86-117">Not supported.</span></span> |
|<span data-ttu-id="59f86-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59f86-118">Application</span></span>                            |<span data-ttu-id="59f86-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59f86-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="59f86-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59f86-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="59f86-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59f86-121">Request headers</span></span>

| <span data-ttu-id="59f86-122">Nome</span><span class="sxs-lookup"><span data-stu-id="59f86-122">Name</span></span>           | <span data-ttu-id="59f86-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f86-123">Type</span></span>    | <span data-ttu-id="59f86-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f86-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="59f86-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="59f86-125">Authorization</span></span>  | <span data-ttu-id="59f86-126">string</span><span class="sxs-lookup"><span data-stu-id="59f86-126">string</span></span>  | <span data-ttu-id="59f86-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59f86-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59f86-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59f86-129">Request body</span></span>

<span data-ttu-id="59f86-130">No corpo da solicitação, fornecem um objeto JSON com o parâmetro a seguir.</span><span class="sxs-lookup"><span data-stu-id="59f86-130">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="59f86-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59f86-131">Parameter</span></span>     | <span data-ttu-id="59f86-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f86-132">Type</span></span>      | <span data-ttu-id="59f86-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f86-133">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="59f86-134">critérios</span><span class="sxs-lookup"><span data-stu-id="59f86-134">criteria</span></span>       |[<span data-ttu-id="59f86-135">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="59f86-135">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="59f86-136">Reinicie os critérios</span><span class="sxs-lookup"><span data-stu-id="59f86-136">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="59f86-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f86-137">Response</span></span>

<span data-ttu-id="59f86-138">Se tiver êxito, retorna um `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="59f86-138">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="59f86-139">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f86-139">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59f86-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59f86-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="59f86-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59f86-141">Request</span></span>
<span data-ttu-id="59f86-142">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="59f86-142">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="59f86-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f86-143">Response</span></span>
<span data-ttu-id="59f86-144">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="59f86-144">The following is an example of a response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
