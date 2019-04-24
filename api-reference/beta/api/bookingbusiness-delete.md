---
title: Excluir bookingBusiness
description: Excluir um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 88f07b46231a942098a157f00097393d60253982
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462404"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="7590e-103">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="7590e-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7590e-104">Excluir um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="7590e-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7590e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7590e-105">Permissions</span></span>
<span data-ttu-id="7590e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7590e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7590e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7590e-108">Permission type</span></span>      | <span data-ttu-id="7590e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7590e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7590e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7590e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7590e-111">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="7590e-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7590e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7590e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7590e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7590e-113">Not supported.</span></span>   |
|<span data-ttu-id="7590e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7590e-114">Application</span></span> | <span data-ttu-id="7590e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7590e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7590e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7590e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="7590e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7590e-117">Request headers</span></span>
| <span data-ttu-id="7590e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7590e-118">Name</span></span>       | <span data-ttu-id="7590e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7590e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7590e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7590e-120">Authorization</span></span>  | <span data-ttu-id="7590e-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7590e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7590e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7590e-122">Request body</span></span>
<span data-ttu-id="7590e-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7590e-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7590e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7590e-124">Response</span></span>
<span data-ttu-id="7590e-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7590e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7590e-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7590e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7590e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7590e-128">Request</span></span>
<span data-ttu-id="7590e-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7590e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="7590e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7590e-130">Response</span></span>
<span data-ttu-id="7590e-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7590e-131">The following is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
