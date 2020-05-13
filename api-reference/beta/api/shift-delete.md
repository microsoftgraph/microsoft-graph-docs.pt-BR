---
title: Excluir Shift
description: Exclui uma alteração do cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0ee4a22d2fc4d206e9ded8419c7fb3317255ece
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "42453315"
---
# <a name="delete-shift"></a><span data-ttu-id="4ea03-103">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="4ea03-103">Delete shift</span></span>

<span data-ttu-id="4ea03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea03-105">Exclui uma [alteração](../resources/shift.md) do cronograma.</span><span class="sxs-lookup"><span data-stu-id="4ea03-105">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ea03-106">Permissions</span></span>

<span data-ttu-id="4ea03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ea03-109">Permission type</span></span>      | <span data-ttu-id="4ea03-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ea03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ea03-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ea03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ea03-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea03-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ea03-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ea03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ea03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea03-114">Not supported.</span></span>    |
|<span data-ttu-id="4ea03-115">Application</span><span class="sxs-lookup"><span data-stu-id="4ea03-115">Application</span></span> | <span data-ttu-id="4ea03-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="4ea03-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="4ea03-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="4ea03-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="4ea03-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4ea03-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4ea03-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="4ea03-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4ea03-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea03-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="4ea03-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea03-121">Request headers</span></span>

| <span data-ttu-id="4ea03-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ea03-122">Header</span></span>       | <span data-ttu-id="4ea03-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4ea03-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ea03-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ea03-124">Authorization</span></span>  | <span data-ttu-id="4ea03-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ea03-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ea03-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea03-127">Request body</span></span>
<span data-ttu-id="4ea03-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ea03-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea03-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea03-129">Response</span></span>

<span data-ttu-id="4ea03-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea03-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea03-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ea03-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4ea03-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea03-133">Request</span></span>

<span data-ttu-id="4ea03-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ea03-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ea03-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea03-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="4ea03-136">C#</span><span class="sxs-lookup"><span data-stu-id="4ea03-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ea03-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ea03-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ea03-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ea03-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ea03-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea03-139">Response</span></span>

<span data-ttu-id="4ea03-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea03-140">The following is an example of the response.</span></span> 

><span data-ttu-id="4ea03-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ea03-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
