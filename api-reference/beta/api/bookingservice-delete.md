---
title: Excluir bookingService
description: Exclua um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a541796fbfa500cc6d99205598042818b4aa47ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461665"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="97c07-103">Excluir bookingService</span><span class="sxs-lookup"><span data-stu-id="97c07-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97c07-104">Exclua um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="97c07-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="97c07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97c07-105">Permissions</span></span>
<span data-ttu-id="97c07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97c07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97c07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97c07-108">Permission type</span></span>      | <span data-ttu-id="97c07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97c07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97c07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97c07-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="97c07-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="97c07-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="97c07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97c07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97c07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97c07-113">Not supported.</span></span>   |
|<span data-ttu-id="97c07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97c07-114">Application</span></span> | <span data-ttu-id="97c07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97c07-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="97c07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97c07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="97c07-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97c07-117">Request headers</span></span>
| <span data-ttu-id="97c07-118">Nome</span><span class="sxs-lookup"><span data-stu-id="97c07-118">Name</span></span>       | <span data-ttu-id="97c07-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c07-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97c07-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="97c07-120">Authorization</span></span>  | <span data-ttu-id="97c07-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="97c07-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="97c07-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97c07-122">Request body</span></span>
<span data-ttu-id="97c07-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97c07-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="97c07-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c07-124">Response</span></span>
<span data-ttu-id="97c07-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97c07-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97c07-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97c07-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97c07-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97c07-128">Request</span></span>
<span data-ttu-id="97c07-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97c07-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="97c07-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c07-130">Response</span></span>
<span data-ttu-id="97c07-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97c07-131">The following is an example of the response.</span></span> <span data-ttu-id="97c07-132">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="97c07-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="97c07-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97c07-133">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
