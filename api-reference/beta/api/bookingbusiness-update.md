---
title: Atualizar bookingbusiness
description: Atualiza as propriedades de um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: fc86060e3d24039286fe679fef83f419a54f42ac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322261"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="4df45-103">Atualizar bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="4df45-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4df45-104">Atualiza as propriedades de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="4df45-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4df45-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4df45-105">Permissions</span></span>
<span data-ttu-id="4df45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4df45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4df45-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4df45-108">Permission type</span></span>      | <span data-ttu-id="4df45-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4df45-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4df45-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4df45-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4df45-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="4df45-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4df45-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4df45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4df45-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4df45-113">Not supported.</span></span>   |
|<span data-ttu-id="4df45-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4df45-114">Application</span></span> | <span data-ttu-id="4df45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4df45-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4df45-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4df45-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="4df45-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4df45-117">Optional request headers</span></span>
| <span data-ttu-id="4df45-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4df45-118">Name</span></span>       | <span data-ttu-id="4df45-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4df45-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4df45-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4df45-120">Authorization</span></span>  | <span data-ttu-id="4df45-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4df45-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4df45-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4df45-122">Request body</span></span>
<span data-ttu-id="4df45-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4df45-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4df45-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4df45-126">Property</span></span>     | <span data-ttu-id="4df45-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4df45-127">Type</span></span>   |<span data-ttu-id="4df45-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4df45-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4df45-129">address</span><span class="sxs-lookup"><span data-stu-id="4df45-129">address</span></span>|[<span data-ttu-id="4df45-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4df45-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="4df45-131">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="4df45-131">The street address of the business.</span></span>|
|<span data-ttu-id="4df45-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="4df45-132">businessHours</span></span>|<span data-ttu-id="4df45-133">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="4df45-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="4df45-134">As horas de operação da empresa.</span><span class="sxs-lookup"><span data-stu-id="4df45-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="4df45-135">businesstype</span><span class="sxs-lookup"><span data-stu-id="4df45-135">businessType</span></span>|<span data-ttu-id="4df45-136">String</span><span class="sxs-lookup"><span data-stu-id="4df45-136">String</span></span>|<span data-ttu-id="4df45-137">O tipo de negócio.</span><span class="sxs-lookup"><span data-stu-id="4df45-137">The type of business.</span></span>|
|<span data-ttu-id="4df45-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="4df45-138">defaultCurrencyIso</span></span>|<span data-ttu-id="4df45-139">String</span><span class="sxs-lookup"><span data-stu-id="4df45-139">String</span></span>|<span data-ttu-id="4df45-140">O código da moeda na qual a empresa opera em reservas da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4df45-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="4df45-141">displayName</span><span class="sxs-lookup"><span data-stu-id="4df45-141">displayName</span></span>|<span data-ttu-id="4df45-142">String</span><span class="sxs-lookup"><span data-stu-id="4df45-142">String</span></span>|<span data-ttu-id="4df45-143">Um nome para a empresa que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="4df45-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="4df45-144">email</span><span class="sxs-lookup"><span data-stu-id="4df45-144">email</span></span>|<span data-ttu-id="4df45-145">String</span><span class="sxs-lookup"><span data-stu-id="4df45-145">String</span></span>|<span data-ttu-id="4df45-146">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="4df45-146">The email address for the business.</span></span>|
|<span data-ttu-id="4df45-147">phone</span><span class="sxs-lookup"><span data-stu-id="4df45-147">phone</span></span>|<span data-ttu-id="4df45-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4df45-148">String</span></span>|<span data-ttu-id="4df45-149">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="4df45-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="4df45-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4df45-150">schedulingPolicy</span></span>|[<span data-ttu-id="4df45-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4df45-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="4df45-152">Especifica como as reservas podem ser criadas para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="4df45-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="4df45-153">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="4df45-153">webSiteUrl</span></span>|<span data-ttu-id="4df45-154">String</span><span class="sxs-lookup"><span data-stu-id="4df45-154">String</span></span>|<span data-ttu-id="4df45-155">A URL do site da empresa.</span><span class="sxs-lookup"><span data-stu-id="4df45-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="4df45-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="4df45-156">Response</span></span>
<span data-ttu-id="4df45-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4df45-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4df45-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4df45-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4df45-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4df45-160">Request</span></span>
<span data-ttu-id="4df45-161">O exemplo a seguir atualiza o endereço de email comercial e a política de agendamento, para alterar o intervalo de tempo de reserva padrão de negócios para uma hora e para a reserva antecipada até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="4df45-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="4df45-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="4df45-162">Response</span></span>
<span data-ttu-id="4df45-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4df45-163">The following is an example of the response.</span></span> <span data-ttu-id="4df45-164">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4df45-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4df45-165">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4df45-165">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
