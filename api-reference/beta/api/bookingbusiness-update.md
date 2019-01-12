---
title: Atualizar bookingbusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3f20d466614e35cce701999fabfb631e081a02ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991332"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="7f4ce-104">Atualizar bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="7f4ce-104">Update bookingbusiness</span></span>

 > <span data-ttu-id="7f4ce-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f4ce-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="7f4ce-107">Atualize as propriedades de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="7f4ce-107">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f4ce-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f4ce-108">Permissions</span></span>
<span data-ttu-id="7f4ce-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f4ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f4ce-111">Permission type</span></span>      | <span data-ttu-id="7f4ce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f4ce-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f4ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f4ce-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f4ce-114">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7f4ce-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7f4ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f4ce-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-116">Not supported.</span></span>   |
|<span data-ttu-id="7f4ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f4ce-117">Application</span></span> | <span data-ttu-id="7f4ce-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="7f4ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f4ce-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="7f4ce-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7f4ce-120">Optional request headers</span></span>
| <span data-ttu-id="7f4ce-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7f4ce-121">Name</span></span>       | <span data-ttu-id="7f4ce-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f4ce-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7f4ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f4ce-123">Authorization</span></span>  | <span data-ttu-id="7f4ce-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7f4ce-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f4ce-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f4ce-125">Request body</span></span>
<span data-ttu-id="7f4ce-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7f4ce-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f4ce-129">Property</span></span>     | <span data-ttu-id="7f4ce-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f4ce-130">Type</span></span>   |<span data-ttu-id="7f4ce-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f4ce-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f4ce-132">address</span><span class="sxs-lookup"><span data-stu-id="7f4ce-132">address</span></span>|[<span data-ttu-id="7f4ce-133">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7f4ce-133">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="7f4ce-134">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-134">The street address of the business.</span></span>|
|<span data-ttu-id="7f4ce-135">businessHours</span><span class="sxs-lookup"><span data-stu-id="7f4ce-135">businessHours</span></span>|<span data-ttu-id="7f4ce-136">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="7f4ce-136">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="7f4ce-137">Os horários de operação para a empresa.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-137">The hours of operation for the business.</span></span>|
|<span data-ttu-id="7f4ce-138">businessType</span><span class="sxs-lookup"><span data-stu-id="7f4ce-138">businessType</span></span>|<span data-ttu-id="7f4ce-139">String</span><span class="sxs-lookup"><span data-stu-id="7f4ce-139">String</span></span>|<span data-ttu-id="7f4ce-140">O tipo de negócio.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-140">The type of business.</span></span>|
|<span data-ttu-id="7f4ce-141">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="7f4ce-141">defaultCurrencyIso</span></span>|<span data-ttu-id="7f4ce-142">String</span><span class="sxs-lookup"><span data-stu-id="7f4ce-142">String</span></span>|<span data-ttu-id="7f4ce-143">O código para a moeda que a empresa opera em Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-143">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="7f4ce-144">displayName</span><span class="sxs-lookup"><span data-stu-id="7f4ce-144">displayName</span></span>|<span data-ttu-id="7f4ce-145">String</span><span class="sxs-lookup"><span data-stu-id="7f4ce-145">String</span></span>|<span data-ttu-id="7f4ce-146">Um nome para a empresa que interage com os clientes.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-146">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="7f4ce-147">email</span><span class="sxs-lookup"><span data-stu-id="7f4ce-147">email</span></span>|<span data-ttu-id="7f4ce-148">String</span><span class="sxs-lookup"><span data-stu-id="7f4ce-148">String</span></span>|<span data-ttu-id="7f4ce-149">O endereço de email para a empresa.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-149">The email address for the business.</span></span>|
|<span data-ttu-id="7f4ce-150">phone</span><span class="sxs-lookup"><span data-stu-id="7f4ce-150">phone</span></span>|<span data-ttu-id="7f4ce-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f4ce-151">String</span></span>|<span data-ttu-id="7f4ce-152">O número de telefone para a empresa.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-152">The telephone number for the business.</span></span>|
|<span data-ttu-id="7f4ce-153">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7f4ce-153">schedulingPolicy</span></span>|[<span data-ttu-id="7f4ce-154">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7f4ce-154">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="7f4ce-155">Especifica como reservas podem ser criadas para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-155">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="7f4ce-156">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="7f4ce-156">webSiteUrl</span></span>|<span data-ttu-id="7f4ce-157">String</span><span class="sxs-lookup"><span data-stu-id="7f4ce-157">String</span></span>|<span data-ttu-id="7f4ce-158">A URL do site da web de negócios.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-158">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="7f4ce-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f4ce-159">Response</span></span>
<span data-ttu-id="7f4ce-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f4ce-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f4ce-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f4ce-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f4ce-163">Request</span></span>
<span data-ttu-id="7f4ce-164">O exemplo a seguir atualiza o endereço de email comercial e o agendamento de política, para alterar o intervalo de tempo de reserva de padrão de negócios para uma hora e Avançar reserva até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-164">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7f4ce-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f4ce-165">Response</span></span>
<span data-ttu-id="7f4ce-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-166">The following is an example of the response.</span></span> <span data-ttu-id="7f4ce-167">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7f4ce-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f4ce-168">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
