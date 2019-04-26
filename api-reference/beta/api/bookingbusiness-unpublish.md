---
title: 'bookingBusiness: cancelar publicação'
description: Tornar a página de agendamento dessa empresa não disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 11ef80e416c1c8ffb85170c6e3171fc003bf937b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322563"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="a8ddc-103">bookingBusiness: cancelar publicação</span><span class="sxs-lookup"><span data-stu-id="a8ddc-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8ddc-104">Tornar a página de agendamento dessa empresa não disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="a8ddc-105">Defina a \*\*\*\* Propriedade IsPublished como false e a propriedade **publicUrl** como NULL.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8ddc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8ddc-106">Permissions</span></span>
<span data-ttu-id="a8ddc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8ddc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8ddc-109">Permission type</span></span>      | <span data-ttu-id="a8ddc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8ddc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8ddc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8ddc-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a8ddc-112">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="a8ddc-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a8ddc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8ddc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8ddc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-114">Not supported.</span></span>   |
|<span data-ttu-id="a8ddc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8ddc-115">Application</span></span> | <span data-ttu-id="a8ddc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a8ddc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8ddc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="a8ddc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8ddc-118">Request headers</span></span>
| <span data-ttu-id="a8ddc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a8ddc-119">Name</span></span>       | <span data-ttu-id="a8ddc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8ddc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8ddc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8ddc-121">Authorization</span></span>  | <span data-ttu-id="a8ddc-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a8ddc-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8ddc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8ddc-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a8ddc-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8ddc-124">Response</span></span>
<span data-ttu-id="a8ddc-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8ddc-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8ddc-127">Example</span></span>
<span data-ttu-id="a8ddc-128">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8ddc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8ddc-129">Request</span></span>
<span data-ttu-id="a8ddc-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="a8ddc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8ddc-131">Response</span></span>
<span data-ttu-id="a8ddc-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8ddc-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
