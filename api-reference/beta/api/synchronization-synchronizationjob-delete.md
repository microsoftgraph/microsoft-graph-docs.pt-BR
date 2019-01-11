---
title: Excluir synchronizationJob
description: Interromper o trabalho de sincronização e excluir permanentemente todo o estado associado a ela. Sincronizadas contas são deixadas como-é.
localization_priority: Normal
ms.openlocfilehash: 95a7d52e9e6fba9bc3f528aedfc5a082d459a003
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835683"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="c2035-104">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="c2035-104">Delete synchronizationJob</span></span>

> <span data-ttu-id="c2035-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2035-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2035-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2035-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2035-107">Interromper o trabalho de sincronização e excluir permanentemente todo o estado associado a ela.</span><span class="sxs-lookup"><span data-stu-id="c2035-107">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="c2035-108">Sincronizadas contas são deixadas como-é.</span><span class="sxs-lookup"><span data-stu-id="c2035-108">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2035-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="c2035-109">Permissions</span></span>
<span data-ttu-id="c2035-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2035-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2035-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2035-112">Permission type</span></span>                        | <span data-ttu-id="c2035-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2035-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2035-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2035-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="c2035-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2035-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c2035-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2035-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c2035-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2035-117">Not supported.</span></span>  |
|<span data-ttu-id="c2035-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2035-118">Application</span></span>                            |<span data-ttu-id="c2035-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2035-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c2035-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2035-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="c2035-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2035-121">Request headers</span></span>

| <span data-ttu-id="c2035-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c2035-122">Name</span></span>           | <span data-ttu-id="c2035-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2035-123">Type</span></span>    | <span data-ttu-id="c2035-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2035-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c2035-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2035-125">Authorization</span></span>  | <span data-ttu-id="c2035-126">string</span><span class="sxs-lookup"><span data-stu-id="c2035-126">string</span></span>  | <span data-ttu-id="c2035-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2035-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2035-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2035-129">Request body</span></span>

<span data-ttu-id="c2035-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2035-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2035-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2035-131">Response</span></span>

<span data-ttu-id="c2035-132">Se tiver êxito, retorna um `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="c2035-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="c2035-133">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2035-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2035-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2035-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2035-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2035-135">Request</span></span>
<span data-ttu-id="c2035-136">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2035-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="c2035-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2035-137">Response</span></span>
<span data-ttu-id="c2035-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2035-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
