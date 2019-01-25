---
title: Excluir bookingCustomer
description: Exclua o objeto bookingCustomer especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 767dea301d554e2ec0131d373b2206b0ef87db6a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525910"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="78383-103">Excluir bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="78383-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78383-104">Exclua o objeto especificado [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="78383-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="78383-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="78383-105">Permissions</span></span>
<span data-ttu-id="78383-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78383-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78383-108">Permission type</span></span>      | <span data-ttu-id="78383-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78383-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78383-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78383-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78383-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="78383-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="78383-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78383-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78383-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78383-113">Not supported.</span></span>   |
|<span data-ttu-id="78383-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78383-114">Application</span></span> | <span data-ttu-id="78383-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78383-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="78383-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78383-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="78383-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78383-117">Request headers</span></span>
| <span data-ttu-id="78383-118">Nome</span><span class="sxs-lookup"><span data-stu-id="78383-118">Name</span></span>       | <span data-ttu-id="78383-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="78383-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78383-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="78383-120">Authorization</span></span>  | <span data-ttu-id="78383-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="78383-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="78383-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78383-122">Request body</span></span>
<span data-ttu-id="78383-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78383-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="78383-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="78383-124">Response</span></span>
<span data-ttu-id="78383-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78383-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78383-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78383-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78383-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78383-128">Request</span></span>
<span data-ttu-id="78383-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78383-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="78383-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="78383-130">Response</span></span>
<span data-ttu-id="78383-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78383-131">The following is an example of the response.</span></span> <span data-ttu-id="78383-132">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="78383-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="78383-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78383-133">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
