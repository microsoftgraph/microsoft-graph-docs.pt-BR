---
title: Excluir timeCard
description: Exclua uma instância timeCard na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f87fe8145d65793b33dc539ed1db235a7e09aebf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787839"
---
# <a name="delete-timecard"></a><span data-ttu-id="32189-103">Excluir timeCard</span><span class="sxs-lookup"><span data-stu-id="32189-103">Delete timeCard</span></span>

<span data-ttu-id="32189-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32189-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32189-105">[Exclua uma instância de cartão](../resources/timeCard.md) de tempo em um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="32189-105">Delete a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="32189-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="32189-106">Permissions</span></span>

<span data-ttu-id="32189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32189-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32189-109">Permission type</span></span>      | <span data-ttu-id="32189-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32189-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32189-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32189-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32189-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32189-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="32189-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32189-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32189-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32189-114">Not supported.</span></span>    |
|<span data-ttu-id="32189-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32189-115">Application</span></span> | <span data-ttu-id="32189-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="32189-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="32189-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="32189-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="32189-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32189-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="32189-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32189-119">Request headers</span></span>

| <span data-ttu-id="32189-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32189-120">Header</span></span>       | <span data-ttu-id="32189-121">Valor</span><span class="sxs-lookup"><span data-stu-id="32189-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32189-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="32189-122">Authorization</span></span>  | <span data-ttu-id="32189-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32189-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="32189-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="32189-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="32189-126">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="32189-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="32189-127">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32189-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32189-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32189-128">Request body</span></span>
<span data-ttu-id="32189-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32189-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32189-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="32189-130">Response</span></span>

<span data-ttu-id="32189-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32189-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32189-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32189-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="32189-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32189-133">Request</span></span>
<span data-ttu-id="32189-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32189-134">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```

### <a name="response"></a><span data-ttu-id="32189-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32189-135">Response</span></span>

<span data-ttu-id="32189-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32189-136">The following is an example of the response.</span></span> 

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
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
