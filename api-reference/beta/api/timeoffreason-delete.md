---
title: Excluir timeOffReason
description: Marque uma timeOffReason como inativa definindo a propriedade IsActive.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e5768df9f0aa039c8eec8d17fb8e83afa0ca9214
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055730"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="14ec2-103">Excluir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="14ec2-103">Delete timeOffReason</span></span>

<span data-ttu-id="14ec2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14ec2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14ec2-105">Marque uma [timeOffReason](../resources/timeoffreason.md) como inativa definindo a propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="14ec2-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="14ec2-106">Cada equipe deve incluir pelo menos um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="14ec2-106">Every team must include at least one **timeOffReason**.</span></span>

<span data-ttu-id="14ec2-107">Este método não remove a instância especificada do **timeOffReason** .</span><span class="sxs-lookup"><span data-stu-id="14ec2-107">This method does not remove the specified **timeOffReason** instance.</span></span> <span data-ttu-id="14ec2-108">as instâncias do [timeOffItem](../resources/timeoffitem.md) que foram atribuídas essa razão permanecem atribuídas a esse motivo.</span><span class="sxs-lookup"><span data-stu-id="14ec2-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="14ec2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="14ec2-109">Permissions</span></span>

<span data-ttu-id="14ec2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ec2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ec2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14ec2-112">Permission type</span></span>      | <span data-ttu-id="14ec2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14ec2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14ec2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14ec2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="14ec2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ec2-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14ec2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14ec2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ec2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14ec2-117">Not supported.</span></span>    |
|<span data-ttu-id="14ec2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14ec2-118">Application</span></span> | <span data-ttu-id="14ec2-119">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="14ec2-119">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="14ec2-120">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="14ec2-120">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="14ec2-121">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="14ec2-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="14ec2-122">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="14ec2-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="14ec2-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14ec2-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="14ec2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14ec2-124">Request headers</span></span>

| <span data-ttu-id="14ec2-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14ec2-125">Header</span></span>       | <span data-ttu-id="14ec2-126">Valor</span><span class="sxs-lookup"><span data-stu-id="14ec2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14ec2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="14ec2-127">Authorization</span></span>  | <span data-ttu-id="14ec2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14ec2-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14ec2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14ec2-130">Request body</span></span>
<span data-ttu-id="14ec2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14ec2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14ec2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ec2-132">Response</span></span>

<span data-ttu-id="14ec2-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14ec2-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14ec2-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14ec2-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="14ec2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14ec2-136">Request</span></span>

<span data-ttu-id="14ec2-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14ec2-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14ec2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="14ec2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="14ec2-139">C#</span><span class="sxs-lookup"><span data-stu-id="14ec2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14ec2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14ec2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14ec2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14ec2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14ec2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ec2-142">Response</span></span>

<span data-ttu-id="14ec2-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14ec2-143">The following is an example of the response.</span></span> 

><span data-ttu-id="14ec2-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14ec2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


