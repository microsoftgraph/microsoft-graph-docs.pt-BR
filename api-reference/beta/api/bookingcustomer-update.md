---
title: Atualizar bookingcustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a22568347e887a9c0ddfc000123e3413d544c7fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990507"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="09cba-104">Atualizar bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="09cba-104">Update bookingcustomer</span></span>

 > <span data-ttu-id="09cba-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="09cba-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09cba-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="09cba-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="09cba-107">Atualize as propriedades de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="09cba-107">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="09cba-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="09cba-108">Permissions</span></span>
<span data-ttu-id="09cba-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09cba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09cba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09cba-111">Permission type</span></span>      | <span data-ttu-id="09cba-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09cba-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09cba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09cba-113">Delegated (work or school account)</span></span> | <span data-ttu-id="09cba-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="09cba-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="09cba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09cba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09cba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09cba-116">Not supported.</span></span>   |
|<span data-ttu-id="09cba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09cba-117">Application</span></span> | <span data-ttu-id="09cba-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09cba-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="09cba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09cba-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="09cba-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="09cba-120">Optional request headers</span></span>
| <span data-ttu-id="09cba-121">Nome</span><span class="sxs-lookup"><span data-stu-id="09cba-121">Name</span></span>       | <span data-ttu-id="09cba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="09cba-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="09cba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09cba-123">Authorization</span></span>  | <span data-ttu-id="09cba-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="09cba-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="09cba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09cba-125">Request body</span></span>
<span data-ttu-id="09cba-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="09cba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="09cba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09cba-129">Property</span></span>     | <span data-ttu-id="09cba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="09cba-130">Type</span></span>   |<span data-ttu-id="09cba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="09cba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09cba-132">displayName</span><span class="sxs-lookup"><span data-stu-id="09cba-132">displayName</span></span>|<span data-ttu-id="09cba-133">String</span><span class="sxs-lookup"><span data-stu-id="09cba-133">String</span></span>|<span data-ttu-id="09cba-134">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="09cba-134">The name of the customer.</span></span>|
|<span data-ttu-id="09cba-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="09cba-135">emailAddress</span></span>|<span data-ttu-id="09cba-136">String</span><span class="sxs-lookup"><span data-stu-id="09cba-136">String</span></span>|<span data-ttu-id="09cba-137">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="09cba-137">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="09cba-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="09cba-138">Response</span></span>
<span data-ttu-id="09cba-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09cba-139">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09cba-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09cba-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09cba-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09cba-141">Request</span></span>
<span data-ttu-id="09cba-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09cba-142">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="09cba-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="09cba-143">Response</span></span>
<span data-ttu-id="09cba-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09cba-144">The following is an example of the response.</span></span> <span data-ttu-id="09cba-145">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="09cba-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="09cba-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09cba-146">All of the properties will be returned from an actual call.</span></span>
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
