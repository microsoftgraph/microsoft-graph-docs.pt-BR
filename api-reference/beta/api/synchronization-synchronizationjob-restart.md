---
title: Reinicie o synchronizationJob
description: Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório. Opcionalmente limpa o estado de sincronização existente e erros anteriores.
localization_priority: Normal
ms.openlocfilehash: 154ae4234eea6fb3499d36720e71b40cac727f9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841024"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="f8070-104">Reinicie o synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f8070-104">Restart synchronizationJob</span></span>

> <span data-ttu-id="f8070-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f8070-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8070-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f8070-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8070-107">Reinicie o trabalho de sincronização, forçando-o a reprocessar todos os objetos no diretório.</span><span class="sxs-lookup"><span data-stu-id="f8070-107">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="f8070-108">Opcionalmente limpa o estado de sincronização existente e erros anteriores.</span><span class="sxs-lookup"><span data-stu-id="f8070-108">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8070-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="f8070-109">Permissions</span></span>
<span data-ttu-id="f8070-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8070-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8070-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8070-112">Permission type</span></span>                        | <span data-ttu-id="f8070-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8070-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8070-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8070-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="f8070-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8070-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f8070-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8070-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f8070-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8070-117">Not supported.</span></span> |
|<span data-ttu-id="f8070-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8070-118">Application</span></span>                            |<span data-ttu-id="f8070-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8070-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f8070-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8070-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="f8070-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8070-121">Request headers</span></span>

| <span data-ttu-id="f8070-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f8070-122">Name</span></span>           | <span data-ttu-id="f8070-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8070-123">Type</span></span>    | <span data-ttu-id="f8070-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8070-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f8070-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8070-125">Authorization</span></span>  | <span data-ttu-id="f8070-126">string</span><span class="sxs-lookup"><span data-stu-id="f8070-126">string</span></span>  | <span data-ttu-id="f8070-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8070-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8070-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8070-129">Request body</span></span>

<span data-ttu-id="f8070-130">No corpo da solicitação, fornecem um objeto JSON com o parâmetro a seguir.</span><span class="sxs-lookup"><span data-stu-id="f8070-130">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="f8070-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f8070-131">Parameter</span></span>     | <span data-ttu-id="f8070-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8070-132">Type</span></span>      | <span data-ttu-id="f8070-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8070-133">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f8070-134">critérios</span><span class="sxs-lookup"><span data-stu-id="f8070-134">criteria</span></span>       |[<span data-ttu-id="f8070-135">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="f8070-135">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="f8070-136">Reinicie os critérios</span><span class="sxs-lookup"><span data-stu-id="f8070-136">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="f8070-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8070-137">Response</span></span>

<span data-ttu-id="f8070-138">Se tiver êxito, retorna um `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="f8070-138">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="f8070-139">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8070-139">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8070-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8070-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f8070-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8070-141">Request</span></span>
<span data-ttu-id="f8070-142">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8070-142">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f8070-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8070-143">Response</span></span>
<span data-ttu-id="f8070-144">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f8070-144">The following is an example of a response.</span></span>

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
