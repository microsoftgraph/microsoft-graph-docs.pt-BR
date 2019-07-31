---
title: Atualizar bookingcustomer
description: Atualiza as propriedades de um objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 933f272d8addcaf0528e5c141291d8f81f3ecb43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944959"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="0c059-103">Atualizar bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="0c059-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c059-104">Atualiza as propriedades de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="0c059-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c059-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c059-105">Permissions</span></span>
<span data-ttu-id="0c059-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c059-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c059-108">Permission type</span></span>      | <span data-ttu-id="0c059-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c059-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c059-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c059-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c059-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="0c059-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0c059-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c059-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c059-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c059-113">Not supported.</span></span>   |
|<span data-ttu-id="0c059-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c059-114">Application</span></span> | <span data-ttu-id="0c059-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c059-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0c059-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c059-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0c059-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0c059-117">Optional request headers</span></span>
| <span data-ttu-id="0c059-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0c059-118">Name</span></span>       | <span data-ttu-id="0c059-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c059-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0c059-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c059-120">Authorization</span></span>  | <span data-ttu-id="0c059-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0c059-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c059-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c059-122">Request body</span></span>
<span data-ttu-id="0c059-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0c059-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c059-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c059-126">Property</span></span>     | <span data-ttu-id="0c059-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c059-127">Type</span></span>   |<span data-ttu-id="0c059-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c059-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c059-129">displayName</span><span class="sxs-lookup"><span data-stu-id="0c059-129">displayName</span></span>|<span data-ttu-id="0c059-130">String</span><span class="sxs-lookup"><span data-stu-id="0c059-130">String</span></span>|<span data-ttu-id="0c059-131">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="0c059-131">The name of the customer.</span></span>|
|<span data-ttu-id="0c059-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0c059-132">emailAddress</span></span>|<span data-ttu-id="0c059-133">String</span><span class="sxs-lookup"><span data-stu-id="0c059-133">String</span></span>|<span data-ttu-id="0c059-134">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="0c059-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="0c059-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c059-135">Response</span></span>
<span data-ttu-id="0c059-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCustomer](../resources/bookingcustomer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c059-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c059-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c059-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c059-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c059-138">Request</span></span>
<span data-ttu-id="0c059-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c059-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c059-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c059-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c059-141">C#</span><span class="sxs-lookup"><span data-stu-id="0c059-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c059-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c059-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c059-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0c059-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c059-144">Java</span><span class="sxs-lookup"><span data-stu-id="0c059-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0c059-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c059-145">Response</span></span>
<span data-ttu-id="0c059-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c059-146">The following is an example of the response.</span></span> <span data-ttu-id="0c059-147">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0c059-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0c059-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c059-148">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
