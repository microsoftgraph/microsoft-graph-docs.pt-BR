---
title: Excluir timeOff
description: Exclua uma instância timeOff de um agendamento.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a9f4426815707882cd5e97283e20446034bb2012
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787363"
---
# <a name="delete-timeoff"></a><span data-ttu-id="481ae-103">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="481ae-103">Delete timeOff</span></span>

<span data-ttu-id="481ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="481ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="481ae-105">[Exclua uma instância timeOff](../resources/timeoff.md) de um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="481ae-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="481ae-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="481ae-106">Permissions</span></span>

<span data-ttu-id="481ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="481ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="481ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="481ae-109">Permission type</span></span>      | <span data-ttu-id="481ae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="481ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="481ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="481ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="481ae-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="481ae-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="481ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="481ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="481ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="481ae-114">Not supported.</span></span>    |
|<span data-ttu-id="481ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="481ae-115">Application</span></span> | <span data-ttu-id="481ae-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="481ae-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="481ae-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="481ae-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="481ae-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="481ae-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="481ae-119">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="481ae-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="481ae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="481ae-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="481ae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="481ae-121">Request headers</span></span>

| <span data-ttu-id="481ae-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="481ae-122">Header</span></span>       | <span data-ttu-id="481ae-123">Valor</span><span class="sxs-lookup"><span data-stu-id="481ae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="481ae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="481ae-124">Authorization</span></span>  | <span data-ttu-id="481ae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="481ae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="481ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="481ae-127">Request body</span></span>
<span data-ttu-id="481ae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="481ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="481ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="481ae-129">Response</span></span>

<span data-ttu-id="481ae-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="481ae-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="481ae-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="481ae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="481ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="481ae-133">Request</span></span>

<span data-ttu-id="481ae-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="481ae-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="481ae-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="481ae-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="481ae-136">C#</span><span class="sxs-lookup"><span data-stu-id="481ae-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="481ae-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="481ae-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="481ae-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="481ae-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="481ae-139">Java</span><span class="sxs-lookup"><span data-stu-id="481ae-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="481ae-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="481ae-140">Response</span></span>

<span data-ttu-id="481ae-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="481ae-141">The following is an example of the response.</span></span> 

><span data-ttu-id="481ae-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="481ae-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


