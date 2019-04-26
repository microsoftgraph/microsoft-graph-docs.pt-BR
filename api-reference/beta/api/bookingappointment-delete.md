---
title: Excluir bookingAppointment
description: Excluir um bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 56fb3ad67736a1a754c979ba01aaf647af3992d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322526"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="3a077-103">Excluir bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="3a077-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a077-104">Excluir um [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="3a077-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3a077-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a077-105">Permissions</span></span>
<span data-ttu-id="3a077-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a077-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a077-108">Permission type</span></span>      | <span data-ttu-id="3a077-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a077-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a077-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a077-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a077-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="3a077-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3a077-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a077-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a077-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a077-113">Not supported.</span></span>   |
|<span data-ttu-id="3a077-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a077-114">Application</span></span> | <span data-ttu-id="3a077-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a077-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3a077-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a077-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3a077-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a077-117">Request headers</span></span>
| <span data-ttu-id="3a077-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3a077-118">Name</span></span>       | <span data-ttu-id="3a077-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a077-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a077-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a077-120">Authorization</span></span>  | <span data-ttu-id="3a077-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3a077-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a077-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a077-122">Request body</span></span>
<span data-ttu-id="3a077-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a077-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3a077-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a077-124">Response</span></span>
<span data-ttu-id="3a077-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a077-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a077-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a077-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a077-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a077-128">Request</span></span>
<span data-ttu-id="3a077-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a077-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="3a077-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a077-130">Response</span></span>
<span data-ttu-id="3a077-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a077-131">The following is an example of the response.</span></span> <span data-ttu-id="3a077-132">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3a077-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3a077-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a077-133">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
