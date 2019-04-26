---
title: Excluir bookingCustomer
description: Exclua o objeto bookingCustomer especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 5ff8d9f276164b9b6c1c5b582668123c3dd4eb02
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322364"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="9167d-103">Excluir bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9167d-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9167d-104">Exclua o objeto [bookingCustomer](../resources/bookingcustomer.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="9167d-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9167d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9167d-105">Permissions</span></span>
<span data-ttu-id="9167d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9167d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9167d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9167d-108">Permission type</span></span>      | <span data-ttu-id="9167d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9167d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9167d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9167d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9167d-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="9167d-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9167d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9167d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9167d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9167d-113">Not supported.</span></span>   |
|<span data-ttu-id="9167d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9167d-114">Application</span></span> | <span data-ttu-id="9167d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9167d-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9167d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9167d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9167d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9167d-117">Request headers</span></span>
| <span data-ttu-id="9167d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9167d-118">Name</span></span>       | <span data-ttu-id="9167d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9167d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9167d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9167d-120">Authorization</span></span>  | <span data-ttu-id="9167d-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9167d-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9167d-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9167d-122">Request body</span></span>
<span data-ttu-id="9167d-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9167d-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9167d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="9167d-124">Response</span></span>
<span data-ttu-id="9167d-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9167d-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9167d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9167d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9167d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9167d-128">Request</span></span>
<span data-ttu-id="9167d-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9167d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="9167d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9167d-130">Response</span></span>
<span data-ttu-id="9167d-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9167d-131">The following is an example of the response.</span></span> <span data-ttu-id="9167d-132">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9167d-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9167d-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9167d-133">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
