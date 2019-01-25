---
title: 'bookingBusiness: cancelamento de publicação'
description: Verifique a página de agendamento dessa empresa não está disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0b6c8122d37e5f6cdb1698b0d86295156e3481a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517523"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="a7c56-103">bookingBusiness: cancelamento de publicação</span><span class="sxs-lookup"><span data-stu-id="a7c56-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c56-104">Verifique a página de agendamento dessa empresa não está disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="a7c56-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="a7c56-105">Defina a propriedade **isPublished** como false e a propriedade **publicUrl** como nulo.</span><span class="sxs-lookup"><span data-stu-id="a7c56-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7c56-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7c56-106">Permissions</span></span>
<span data-ttu-id="a7c56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c56-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7c56-109">Permission type</span></span>      | <span data-ttu-id="a7c56-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7c56-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7c56-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7c56-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a7c56-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a7c56-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a7c56-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7c56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7c56-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7c56-114">Not supported.</span></span>   |
|<span data-ttu-id="a7c56-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7c56-115">Application</span></span> | <span data-ttu-id="a7c56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7c56-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a7c56-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7c56-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="a7c56-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c56-118">Request headers</span></span>
| <span data-ttu-id="a7c56-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a7c56-119">Name</span></span>       | <span data-ttu-id="a7c56-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c56-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7c56-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7c56-121">Authorization</span></span>  | <span data-ttu-id="a7c56-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a7c56-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c56-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c56-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a7c56-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7c56-124">Response</span></span>
<span data-ttu-id="a7c56-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7c56-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7c56-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7c56-127">Example</span></span>
<span data-ttu-id="a7c56-128">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a7c56-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a7c56-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7c56-129">Request</span></span>
<span data-ttu-id="a7c56-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7c56-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="a7c56-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7c56-131">Response</span></span>
<span data-ttu-id="a7c56-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7c56-132">The following is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
