---
title: Excluir bookingService
description: Exclua um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 71d96f057c4e1d5282729938a6188bdc2718f96c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322422"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="95c98-103">Excluir bookingService</span><span class="sxs-lookup"><span data-stu-id="95c98-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c98-104">Exclua um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="95c98-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="95c98-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="95c98-105">Permissions</span></span>
<span data-ttu-id="95c98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95c98-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95c98-108">Permission type</span></span>      | <span data-ttu-id="95c98-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95c98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95c98-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95c98-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="95c98-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="95c98-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="95c98-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95c98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95c98-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c98-113">Not supported.</span></span>   |
|<span data-ttu-id="95c98-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95c98-114">Application</span></span> | <span data-ttu-id="95c98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c98-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="95c98-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95c98-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="95c98-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95c98-117">Request headers</span></span>
| <span data-ttu-id="95c98-118">Nome</span><span class="sxs-lookup"><span data-stu-id="95c98-118">Name</span></span>       | <span data-ttu-id="95c98-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c98-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="95c98-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="95c98-120">Authorization</span></span>  | <span data-ttu-id="95c98-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="95c98-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="95c98-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95c98-122">Request body</span></span>
<span data-ttu-id="95c98-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95c98-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="95c98-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c98-124">Response</span></span>
<span data-ttu-id="95c98-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c98-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95c98-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95c98-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95c98-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c98-128">Request</span></span>
<span data-ttu-id="95c98-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="95c98-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="95c98-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c98-130">Response</span></span>
<span data-ttu-id="95c98-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95c98-131">The following is an example of the response.</span></span> <span data-ttu-id="95c98-132">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="95c98-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="95c98-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95c98-133">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
