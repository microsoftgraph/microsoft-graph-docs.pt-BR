---
title: Excluir bookingAppointment
description: Exclua um bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a8abe1961be7e3caf36c9d690497347f42c83fde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513715"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="e226c-103">Excluir bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="e226c-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e226c-104">Exclua um [bookingAppointment](../resources/bookingappointment.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="e226c-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e226c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e226c-105">Permissions</span></span>
<span data-ttu-id="e226c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e226c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e226c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e226c-108">Permission type</span></span>      | <span data-ttu-id="e226c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e226c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e226c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e226c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e226c-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e226c-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e226c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e226c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e226c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e226c-113">Not supported.</span></span>   |
|<span data-ttu-id="e226c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e226c-114">Application</span></span> | <span data-ttu-id="e226c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e226c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e226c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e226c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e226c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e226c-117">Request headers</span></span>
| <span data-ttu-id="e226c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e226c-118">Name</span></span>       | <span data-ttu-id="e226c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e226c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e226c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e226c-120">Authorization</span></span>  | <span data-ttu-id="e226c-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e226c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e226c-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e226c-122">Request body</span></span>
<span data-ttu-id="e226c-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e226c-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e226c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="e226c-124">Response</span></span>
<span data-ttu-id="e226c-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e226c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e226c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e226c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e226c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e226c-128">Request</span></span>
<span data-ttu-id="e226c-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e226c-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="e226c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e226c-130">Response</span></span>
<span data-ttu-id="e226c-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e226c-131">The following is an example of the response.</span></span> <span data-ttu-id="e226c-132">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e226c-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e226c-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e226c-133">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
