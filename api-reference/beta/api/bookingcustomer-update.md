---
title: Atualizar bookingcustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: d28a2a30da1c626c65c65a1dc3cab000a06580d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034685"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="48327-104">Atualizar bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="48327-104">Update bookingcustomer</span></span>

 > <span data-ttu-id="48327-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48327-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48327-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48327-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="48327-107">Atualize as propriedades de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="48327-107">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="48327-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="48327-108">Permissions</span></span>
<span data-ttu-id="48327-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48327-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48327-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48327-111">Permission type</span></span>      | <span data-ttu-id="48327-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48327-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48327-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48327-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48327-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="48327-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="48327-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48327-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48327-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48327-116">Not supported.</span></span>   |
|<span data-ttu-id="48327-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48327-117">Application</span></span> | <span data-ttu-id="48327-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48327-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="48327-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48327-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="48327-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="48327-120">Optional request headers</span></span>
| <span data-ttu-id="48327-121">Nome</span><span class="sxs-lookup"><span data-stu-id="48327-121">Name</span></span>       | <span data-ttu-id="48327-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="48327-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="48327-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48327-123">Authorization</span></span>  | <span data-ttu-id="48327-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="48327-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="48327-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48327-125">Request body</span></span>
<span data-ttu-id="48327-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="48327-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="48327-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48327-129">Property</span></span>     | <span data-ttu-id="48327-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="48327-130">Type</span></span>   |<span data-ttu-id="48327-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="48327-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48327-132">displayName</span><span class="sxs-lookup"><span data-stu-id="48327-132">displayName</span></span>|<span data-ttu-id="48327-133">String</span><span class="sxs-lookup"><span data-stu-id="48327-133">String</span></span>|<span data-ttu-id="48327-134">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="48327-134">The name of the customer.</span></span>|
|<span data-ttu-id="48327-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="48327-135">emailAddress</span></span>|<span data-ttu-id="48327-136">String</span><span class="sxs-lookup"><span data-stu-id="48327-136">String</span></span>|<span data-ttu-id="48327-137">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="48327-137">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="48327-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="48327-138">Response</span></span>
<span data-ttu-id="48327-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48327-139">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48327-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48327-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48327-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48327-141">Request</span></span>
<span data-ttu-id="48327-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48327-142">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="48327-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="48327-143">Response</span></span>
<span data-ttu-id="48327-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48327-144">The following is an example of the response.</span></span> <span data-ttu-id="48327-145">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="48327-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="48327-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48327-146">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->