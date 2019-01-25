---
title: Excluir bookingBusiness
description: Exclua um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 88f07b46231a942098a157f00097393d60253982
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511895"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="9ba07-103">Excluir bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="9ba07-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ba07-104">Exclua um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="9ba07-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ba07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ba07-105">Permissions</span></span>
<span data-ttu-id="9ba07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ba07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ba07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ba07-108">Permission type</span></span>      | <span data-ttu-id="9ba07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ba07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ba07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ba07-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ba07-111">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="9ba07-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9ba07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ba07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ba07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ba07-113">Not supported.</span></span>   |
|<span data-ttu-id="9ba07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ba07-114">Application</span></span> | <span data-ttu-id="9ba07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ba07-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9ba07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ba07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="9ba07-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ba07-117">Request headers</span></span>
| <span data-ttu-id="9ba07-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9ba07-118">Name</span></span>       | <span data-ttu-id="9ba07-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ba07-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ba07-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ba07-120">Authorization</span></span>  | <span data-ttu-id="9ba07-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9ba07-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ba07-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ba07-122">Request body</span></span>
<span data-ttu-id="9ba07-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ba07-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9ba07-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ba07-124">Response</span></span>
<span data-ttu-id="9ba07-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ba07-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ba07-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ba07-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ba07-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ba07-128">Request</span></span>
<span data-ttu-id="9ba07-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ba07-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="9ba07-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ba07-130">Response</span></span>
<span data-ttu-id="9ba07-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ba07-131">The following is an example of the response.</span></span>
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
