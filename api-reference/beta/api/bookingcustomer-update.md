---
title: Atualizar bookingcustomer
description: Atualiza as propriedades de um objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 90de81666335c1825e1d134f9b898ee4b6561664
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461728"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="696d3-103">Atualizar bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="696d3-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="696d3-104">Atualiza as propriedades de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="696d3-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="696d3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="696d3-105">Permissions</span></span>
<span data-ttu-id="696d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="696d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="696d3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="696d3-108">Permission type</span></span>      | <span data-ttu-id="696d3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="696d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="696d3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="696d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="696d3-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="696d3-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="696d3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="696d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="696d3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="696d3-113">Not supported.</span></span>   |
|<span data-ttu-id="696d3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="696d3-114">Application</span></span> | <span data-ttu-id="696d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="696d3-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="696d3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="696d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="696d3-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="696d3-117">Optional request headers</span></span>
| <span data-ttu-id="696d3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="696d3-118">Name</span></span>       | <span data-ttu-id="696d3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="696d3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="696d3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="696d3-120">Authorization</span></span>  | <span data-ttu-id="696d3-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="696d3-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="696d3-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="696d3-122">Request body</span></span>
<span data-ttu-id="696d3-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="696d3-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="696d3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="696d3-126">Property</span></span>     | <span data-ttu-id="696d3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="696d3-127">Type</span></span>   |<span data-ttu-id="696d3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="696d3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="696d3-129">displayName</span><span class="sxs-lookup"><span data-stu-id="696d3-129">displayName</span></span>|<span data-ttu-id="696d3-130">String</span><span class="sxs-lookup"><span data-stu-id="696d3-130">String</span></span>|<span data-ttu-id="696d3-131">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="696d3-131">The name of the customer.</span></span>|
|<span data-ttu-id="696d3-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="696d3-132">emailAddress</span></span>|<span data-ttu-id="696d3-133">String</span><span class="sxs-lookup"><span data-stu-id="696d3-133">String</span></span>|<span data-ttu-id="696d3-134">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="696d3-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="696d3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="696d3-135">Response</span></span>
<span data-ttu-id="696d3-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCustomer](../resources/bookingcustomer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="696d3-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="696d3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="696d3-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="696d3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="696d3-138">Request</span></span>
<span data-ttu-id="696d3-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="696d3-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="696d3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="696d3-140">Response</span></span>
<span data-ttu-id="696d3-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="696d3-141">The following is an example of the response.</span></span> <span data-ttu-id="696d3-142">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="696d3-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="696d3-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="696d3-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
