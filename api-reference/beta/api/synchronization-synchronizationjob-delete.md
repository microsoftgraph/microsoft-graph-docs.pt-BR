---
title: Excluir synchronizationJob
description: Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele. As contas sincronizadas são deixadas como estão.
localization_priority: Normal
ms.openlocfilehash: e199f950e2108a98123db83e35a7a1a75bd8fa3f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335705"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="f4c14-104">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f4c14-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4c14-105">Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="f4c14-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="f4c14-106">As contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="f4c14-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c14-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4c14-107">Permissions</span></span>
<span data-ttu-id="f4c14-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4c14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4c14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4c14-110">Permission type</span></span>                        | <span data-ttu-id="f4c14-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4c14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4c14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4c14-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="f4c14-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c14-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f4c14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4c14-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f4c14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4c14-115">Not supported.</span></span>  |
|<span data-ttu-id="f4c14-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4c14-116">Application</span></span>                            |<span data-ttu-id="f4c14-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4c14-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f4c14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c14-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="f4c14-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c14-119">Request headers</span></span>

| <span data-ttu-id="f4c14-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f4c14-120">Name</span></span>           | <span data-ttu-id="f4c14-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4c14-121">Type</span></span>    | <span data-ttu-id="f4c14-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4c14-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f4c14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4c14-123">Authorization</span></span>  | <span data-ttu-id="f4c14-124">string</span><span class="sxs-lookup"><span data-stu-id="f4c14-124">string</span></span>  | <span data-ttu-id="f4c14-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4c14-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4c14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c14-127">Request body</span></span>

<span data-ttu-id="f4c14-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4c14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c14-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4c14-129">Response</span></span>

<span data-ttu-id="f4c14-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f4c14-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="f4c14-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4c14-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4c14-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4c14-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f4c14-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4c14-133">Request</span></span>
<span data-ttu-id="f4c14-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4c14-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="f4c14-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4c14-135">Response</span></span>
<span data-ttu-id="f4c14-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f4c14-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
