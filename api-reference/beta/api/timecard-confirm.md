---
title: 'timeCard: confirme'
description: Confirme um cartão de ponto específico.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 42ee0d8c1259b31ebf96716ca1c49656af4075f8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787841"
---
# <a name="timecard-confirm"></a><span data-ttu-id="a7413-103">timeCard: confirme</span><span class="sxs-lookup"><span data-stu-id="a7413-103">timeCard: confirm</span></span>

<span data-ttu-id="a7413-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7413-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7413-105">Confirme um [cartão de ponto específico](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="a7413-105">Confirm a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7413-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a7413-106">Permissions</span></span>

<span data-ttu-id="a7413-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7413-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7413-109">Permission type</span></span>      | <span data-ttu-id="a7413-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7413-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7413-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7413-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7413-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7413-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7413-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7413-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7413-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7413-114">Not supported.</span></span>    |
|<span data-ttu-id="a7413-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7413-115">Application</span></span> | <span data-ttu-id="a7413-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="a7413-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a7413-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7413-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="a7413-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7413-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/confirm
```

## <a name="request-headers"></a><span data-ttu-id="a7413-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7413-119">Request headers</span></span>

| <span data-ttu-id="a7413-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7413-120">Header</span></span>       | <span data-ttu-id="a7413-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a7413-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7413-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7413-122">Authorization</span></span>  | <span data-ttu-id="a7413-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7413-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7413-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="a7413-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="a7413-126">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="a7413-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="a7413-127">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a7413-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7413-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7413-128">Request body</span></span>
<span data-ttu-id="a7413-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7413-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7413-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7413-130">Response</span></span>

<span data-ttu-id="a7413-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7413-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7413-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7413-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7413-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7413-133">Request</span></span>
<span data-ttu-id="a7413-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7413-134">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-confirm"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/confirm
```

### <a name="response"></a><span data-ttu-id="a7413-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7413-135">Response</span></span>

<span data-ttu-id="a7413-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7413-136">The following is an example of the response.</span></span> 

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
  "description": "Confirm timecard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
