---
title: Iniciar synchronizationJob
description: Inicie um trabalho de sincronização existente. Se o trabalho estiver em um estado pausado, ele continuará o processamento de alterações do ponto onde foi pausado. Se o trabalho estiver em quarentena, o status de quarentena vai ser limpa.
localization_priority: Normal
ms.openlocfilehash: 478f29d1c49cf6cc820fcc52393f4721ff94caac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826212"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="48068-105">Iniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="48068-105">Start synchronizationJob</span></span>

> <span data-ttu-id="48068-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48068-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48068-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48068-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48068-108">Inicie um trabalho de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="48068-108">Start an existing synchronization job.</span></span> <span data-ttu-id="48068-109">Se o trabalho estiver em um estado pausado, ele continuará o processamento de alterações do ponto onde foi pausado.</span><span class="sxs-lookup"><span data-stu-id="48068-109">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="48068-110">Se o trabalho estiver em quarentena, o status de quarentena vai ser limpa.</span><span class="sxs-lookup"><span data-stu-id="48068-110">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="48068-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="48068-111">Permissions</span></span>
<span data-ttu-id="48068-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48068-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48068-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48068-114">Permission type</span></span>                        | <span data-ttu-id="48068-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48068-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="48068-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48068-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="48068-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48068-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="48068-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48068-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="48068-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48068-119">Not supported.</span></span> |
|<span data-ttu-id="48068-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48068-120">Application</span></span>                            |<span data-ttu-id="48068-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48068-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="48068-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48068-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="48068-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48068-123">Request headers</span></span>

| <span data-ttu-id="48068-124">Nome</span><span class="sxs-lookup"><span data-stu-id="48068-124">Name</span></span>           | <span data-ttu-id="48068-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="48068-125">Type</span></span>    | <span data-ttu-id="48068-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="48068-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="48068-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="48068-127">Authorization</span></span>  | <span data-ttu-id="48068-128">string</span><span class="sxs-lookup"><span data-stu-id="48068-128">string</span></span>  | <span data-ttu-id="48068-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48068-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48068-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48068-131">Request body</span></span>

<span data-ttu-id="48068-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48068-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="48068-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="48068-133">Response</span></span>

<span data-ttu-id="48068-134">Se tiver êxito, retorna um `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="48068-134">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="48068-135">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48068-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48068-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48068-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48068-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48068-137">Request</span></span>
<span data-ttu-id="48068-138">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="48068-138">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="48068-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="48068-139">Response</span></span>
<span data-ttu-id="48068-140">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="48068-140">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
