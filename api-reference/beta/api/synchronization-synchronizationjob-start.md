---
title: Iniciar synchronizationJob
description: Inicie um trabalho de sincronização existente. Se o trabalho estiver em um estado pausado, ele continuará processando as alterações do ponto em que foi pausado. Se o trabalho estiver em quarentena, o status da quarentena será limpo.
localization_priority: Normal
ms.openlocfilehash: dc3afbf958278c7931bb428d9117ae34c3a7562b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335686"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="8cc02-105">Iniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="8cc02-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc02-106">Inicie um trabalho de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="8cc02-106">Start an existing synchronization job.</span></span> <span data-ttu-id="8cc02-107">Se o trabalho estiver em um estado pausado, ele continuará processando as alterações do ponto em que foi pausado.</span><span class="sxs-lookup"><span data-stu-id="8cc02-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="8cc02-108">Se o trabalho estiver em quarentena, o status da quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="8cc02-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc02-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc02-109">Permissions</span></span>
<span data-ttu-id="8cc02-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc02-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc02-112">Permission type</span></span>                        | <span data-ttu-id="8cc02-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc02-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc02-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc02-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="8cc02-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc02-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8cc02-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc02-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8cc02-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc02-117">Not supported.</span></span> |
|<span data-ttu-id="8cc02-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc02-118">Application</span></span>                            |<span data-ttu-id="8cc02-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc02-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8cc02-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc02-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="8cc02-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc02-121">Request headers</span></span>

| <span data-ttu-id="8cc02-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc02-122">Name</span></span>           | <span data-ttu-id="8cc02-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc02-123">Type</span></span>    | <span data-ttu-id="8cc02-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc02-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8cc02-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc02-125">Authorization</span></span>  | <span data-ttu-id="8cc02-126">string</span><span class="sxs-lookup"><span data-stu-id="8cc02-126">string</span></span>  | <span data-ttu-id="8cc02-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc02-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cc02-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc02-129">Request body</span></span>

<span data-ttu-id="8cc02-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8cc02-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="8cc02-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc02-131">Response</span></span>

<span data-ttu-id="8cc02-132">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc02-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="8cc02-133">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc02-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc02-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc02-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8cc02-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc02-135">Request</span></span>
<span data-ttu-id="8cc02-136">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc02-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="8cc02-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc02-137">Response</span></span>
<span data-ttu-id="8cc02-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc02-138">The following is an example of a response.</span></span>
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
  "suppressions": []
}
-->
