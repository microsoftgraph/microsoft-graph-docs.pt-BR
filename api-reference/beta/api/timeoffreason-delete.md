---
title: Excluir timeOffReason
description: Marque uma timeOffReason como inativa definindo a propriedade IsActive.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e71e976167b94d144037d93bf9bb3dff59cc5b7
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154420"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="d9a74-103">Excluir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="d9a74-103">Delete timeOffReason</span></span>

<span data-ttu-id="d9a74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9a74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9a74-105">Marque uma [timeOffReason](../resources/timeoffreason.md) como inativa definindo a propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="d9a74-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="d9a74-106">Cada equipe deve incluir pelo menos um **timeOffReason**.</span><span class="sxs-lookup"><span data-stu-id="d9a74-106">Every team must include at least one **timeOffReason**.</span></span>

<span data-ttu-id="d9a74-107">Este método não remove a instância especificada do **timeOffReason** .</span><span class="sxs-lookup"><span data-stu-id="d9a74-107">This method does not remove the specified **timeOffReason** instance.</span></span> <span data-ttu-id="d9a74-108">as instâncias do [timeOffItem](../resources/timeoffitem.md) que foram atribuídas essa razão permanecem atribuídas a esse motivo.</span><span class="sxs-lookup"><span data-stu-id="d9a74-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9a74-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9a74-109">Permissions</span></span>

<span data-ttu-id="d9a74-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9a74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9a74-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9a74-112">Permission type</span></span>      | <span data-ttu-id="d9a74-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9a74-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9a74-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9a74-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d9a74-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a74-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9a74-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9a74-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9a74-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9a74-117">Not supported.</span></span>    |
|<span data-ttu-id="d9a74-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9a74-118">Application</span></span> | <span data-ttu-id="d9a74-119">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="d9a74-119">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="d9a74-120">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="d9a74-120">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="d9a74-121">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d9a74-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d9a74-122">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d9a74-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9a74-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9a74-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="d9a74-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a74-124">Request headers</span></span>

| <span data-ttu-id="d9a74-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9a74-125">Header</span></span>       | <span data-ttu-id="d9a74-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d9a74-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9a74-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9a74-127">Authorization</span></span>  | <span data-ttu-id="d9a74-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9a74-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9a74-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a74-130">Request body</span></span>
<span data-ttu-id="d9a74-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9a74-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9a74-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a74-132">Response</span></span>

<span data-ttu-id="d9a74-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9a74-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9a74-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9a74-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d9a74-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a74-136">Request</span></span>

<span data-ttu-id="d9a74-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9a74-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9a74-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9a74-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="d9a74-139">C#</span><span class="sxs-lookup"><span data-stu-id="d9a74-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9a74-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9a74-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9a74-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9a74-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9a74-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a74-142">Response</span></span>

<span data-ttu-id="d9a74-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9a74-143">The following is an example of the response.</span></span> 

><span data-ttu-id="d9a74-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9a74-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
