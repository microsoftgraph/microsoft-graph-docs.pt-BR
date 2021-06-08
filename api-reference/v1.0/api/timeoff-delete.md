---
title: Excluir timeOff
description: Exclua uma instância timeOff de um agendamento.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a10dbde99b62cebf99f82c9ac67743943f83a63
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787713"
---
# <a name="delete-timeoff"></a><span data-ttu-id="86ea5-103">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="86ea5-103">Delete timeOff</span></span>

<span data-ttu-id="86ea5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86ea5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86ea5-105">[Exclua uma instância timeOff](../resources/timeoff.md) de um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="86ea5-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86ea5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86ea5-106">Permissions</span></span>

<span data-ttu-id="86ea5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ea5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ea5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86ea5-109">Permission type</span></span>      | <span data-ttu-id="86ea5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86ea5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86ea5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86ea5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86ea5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ea5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86ea5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86ea5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86ea5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86ea5-114">Not supported.</span></span>    |
|<span data-ttu-id="86ea5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86ea5-115">Application</span></span> | <span data-ttu-id="86ea5-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ea5-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="86ea5-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="86ea5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="86ea5-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="86ea5-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="86ea5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86ea5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="86ea5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86ea5-120">Request headers</span></span>

| <span data-ttu-id="86ea5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86ea5-121">Header</span></span>       | <span data-ttu-id="86ea5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86ea5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86ea5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86ea5-123">Authorization</span></span>  | <span data-ttu-id="86ea5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86ea5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86ea5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86ea5-126">Request body</span></span>
<span data-ttu-id="86ea5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86ea5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86ea5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ea5-128">Response</span></span>

<span data-ttu-id="86ea5-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86ea5-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ea5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86ea5-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="86ea5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86ea5-132">Request</span></span>

<span data-ttu-id="86ea5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86ea5-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86ea5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="86ea5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="86ea5-135">C#</span><span class="sxs-lookup"><span data-stu-id="86ea5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86ea5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86ea5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86ea5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86ea5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86ea5-138">Java</span><span class="sxs-lookup"><span data-stu-id="86ea5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="86ea5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ea5-139">Response</span></span>

<span data-ttu-id="86ea5-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86ea5-140">The following is an example of the response.</span></span> 

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
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

