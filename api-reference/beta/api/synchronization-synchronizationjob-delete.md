---
title: Excluir synchronizationJob
description: Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele. As contas sincronizadas são deixadas como estão.
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545211"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="5dff1-104">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5dff1-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dff1-105">Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="5dff1-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="5dff1-106">As contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="5dff1-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dff1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dff1-107">Permissions</span></span>
<span data-ttu-id="5dff1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dff1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dff1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dff1-110">Permission type</span></span>                        | <span data-ttu-id="5dff1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dff1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dff1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dff1-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="5dff1-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dff1-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5dff1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dff1-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5dff1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dff1-115">Not supported.</span></span>  |
|<span data-ttu-id="5dff1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dff1-116">Application</span></span>                            |<span data-ttu-id="5dff1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dff1-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5dff1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dff1-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="5dff1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dff1-119">Request headers</span></span>

| <span data-ttu-id="5dff1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5dff1-120">Name</span></span>           | <span data-ttu-id="5dff1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dff1-121">Type</span></span>    | <span data-ttu-id="5dff1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dff1-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5dff1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dff1-123">Authorization</span></span>  | <span data-ttu-id="5dff1-124">string</span><span class="sxs-lookup"><span data-stu-id="5dff1-124">string</span></span>  | <span data-ttu-id="5dff1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dff1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dff1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dff1-127">Request body</span></span>

<span data-ttu-id="5dff1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5dff1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dff1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dff1-129">Response</span></span>

<span data-ttu-id="5dff1-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5dff1-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="5dff1-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dff1-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dff1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dff1-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5dff1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dff1-133">Request</span></span>
<span data-ttu-id="5dff1-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dff1-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="5dff1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dff1-135">Response</span></span>
<span data-ttu-id="5dff1-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5dff1-136">The following is an example of the response.</span></span> 

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
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
