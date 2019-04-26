---
title: Excluir bookingBusiness
description: Excluir um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 32269e364963d5335d858fa4cce68b279cd8a9c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322513"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="3e821-103">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="3e821-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e821-104">Excluir um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="3e821-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e821-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e821-105">Permissions</span></span>
<span data-ttu-id="3e821-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e821-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e821-108">Permission type</span></span>      | <span data-ttu-id="3e821-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e821-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e821-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e821-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3e821-111">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="3e821-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3e821-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e821-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e821-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e821-113">Not supported.</span></span>   |
|<span data-ttu-id="3e821-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e821-114">Application</span></span> | <span data-ttu-id="3e821-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e821-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3e821-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e821-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="3e821-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e821-117">Request headers</span></span>
| <span data-ttu-id="3e821-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3e821-118">Name</span></span>       | <span data-ttu-id="3e821-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e821-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e821-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e821-120">Authorization</span></span>  | <span data-ttu-id="3e821-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3e821-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e821-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e821-122">Request body</span></span>
<span data-ttu-id="3e821-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e821-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3e821-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e821-124">Response</span></span>
<span data-ttu-id="3e821-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e821-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e821-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e821-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e821-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e821-128">Request</span></span>
<span data-ttu-id="3e821-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e821-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="3e821-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e821-130">Response</span></span>
<span data-ttu-id="3e821-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e821-131">The following is an example of the response.</span></span>
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
