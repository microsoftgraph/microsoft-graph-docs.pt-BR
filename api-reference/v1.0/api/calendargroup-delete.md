---
title: Excluir calendarGroup
description: Exclui um grupo de calendários diferente do grupo de calendários padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3d2a6ca43bc3cc53f4620af6767f1df81ede9816
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443774"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="5c425-103">Excluir calendarGroup</span><span class="sxs-lookup"><span data-stu-id="5c425-103">Delete calendarGroup</span></span>

<span data-ttu-id="5c425-104">Exclui um grupo de calendários diferente do grupo de calendários padrão.</span><span class="sxs-lookup"><span data-stu-id="5c425-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c425-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c425-105">Permissions</span></span>

<span data-ttu-id="5c425-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c425-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c425-108">Permission type</span></span>                        | <span data-ttu-id="5c425-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c425-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5c425-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c425-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c425-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c425-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5c425-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c425-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c425-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c425-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5c425-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c425-114">Application</span></span>                            | <span data-ttu-id="5c425-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c425-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5c425-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c425-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5c425-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c425-117">Request headers</span></span>

| <span data-ttu-id="5c425-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5c425-118">Name</span></span>          | <span data-ttu-id="5c425-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c425-119">Type</span></span>   | <span data-ttu-id="5c425-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c425-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="5c425-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c425-121">Authorization</span></span> | <span data-ttu-id="5c425-122">string</span><span class="sxs-lookup"><span data-stu-id="5c425-122">string</span></span> | <span data-ttu-id="5c425-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c425-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c425-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c425-125">Request body</span></span>

<span data-ttu-id="5c425-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c425-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c425-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c425-127">Response</span></span>

<span data-ttu-id="5c425-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c425-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c425-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c425-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5c425-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c425-131">Request</span></span>

<span data-ttu-id="5c425-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c425-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5c425-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c425-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c425-134">C#</span><span class="sxs-lookup"><span data-stu-id="5c425-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c425-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c425-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c425-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5c425-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c425-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c425-137">Response</span></span>

<span data-ttu-id="5c425-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c425-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
