---
title: Atualizar bookingbusiness
description: Atualize as propriedades de um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dba24dafef030ae53fc83fb06d1cc7b99ed71e81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528799"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="871d7-103">Atualizar bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="871d7-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="871d7-104">Atualize as propriedades de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="871d7-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="871d7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="871d7-105">Permissions</span></span>
<span data-ttu-id="871d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="871d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="871d7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="871d7-108">Permission type</span></span>      | <span data-ttu-id="871d7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="871d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="871d7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="871d7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="871d7-111">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="871d7-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="871d7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="871d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="871d7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="871d7-113">Not supported.</span></span>   |
|<span data-ttu-id="871d7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="871d7-114">Application</span></span> | <span data-ttu-id="871d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="871d7-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="871d7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="871d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="871d7-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="871d7-117">Optional request headers</span></span>
| <span data-ttu-id="871d7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="871d7-118">Name</span></span>       | <span data-ttu-id="871d7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="871d7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="871d7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="871d7-120">Authorization</span></span>  | <span data-ttu-id="871d7-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="871d7-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="871d7-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="871d7-122">Request body</span></span>
<span data-ttu-id="871d7-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="871d7-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="871d7-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="871d7-126">Property</span></span>     | <span data-ttu-id="871d7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="871d7-127">Type</span></span>   |<span data-ttu-id="871d7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="871d7-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="871d7-129">address</span><span class="sxs-lookup"><span data-stu-id="871d7-129">address</span></span>|[<span data-ttu-id="871d7-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="871d7-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="871d7-131">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="871d7-131">The street address of the business.</span></span>|
|<span data-ttu-id="871d7-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="871d7-132">businessHours</span></span>|<span data-ttu-id="871d7-133">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="871d7-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="871d7-134">Os horários de operação para a empresa.</span><span class="sxs-lookup"><span data-stu-id="871d7-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="871d7-135">businessType</span><span class="sxs-lookup"><span data-stu-id="871d7-135">businessType</span></span>|<span data-ttu-id="871d7-136">String</span><span class="sxs-lookup"><span data-stu-id="871d7-136">String</span></span>|<span data-ttu-id="871d7-137">O tipo de negócio.</span><span class="sxs-lookup"><span data-stu-id="871d7-137">The type of business.</span></span>|
|<span data-ttu-id="871d7-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="871d7-138">defaultCurrencyIso</span></span>|<span data-ttu-id="871d7-139">String</span><span class="sxs-lookup"><span data-stu-id="871d7-139">String</span></span>|<span data-ttu-id="871d7-140">O código para a moeda que a empresa opera em Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="871d7-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="871d7-141">displayName</span><span class="sxs-lookup"><span data-stu-id="871d7-141">displayName</span></span>|<span data-ttu-id="871d7-142">String</span><span class="sxs-lookup"><span data-stu-id="871d7-142">String</span></span>|<span data-ttu-id="871d7-143">Um nome para a empresa que interage com os clientes.</span><span class="sxs-lookup"><span data-stu-id="871d7-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="871d7-144">email</span><span class="sxs-lookup"><span data-stu-id="871d7-144">email</span></span>|<span data-ttu-id="871d7-145">String</span><span class="sxs-lookup"><span data-stu-id="871d7-145">String</span></span>|<span data-ttu-id="871d7-146">O endereço de email para a empresa.</span><span class="sxs-lookup"><span data-stu-id="871d7-146">The email address for the business.</span></span>|
|<span data-ttu-id="871d7-147">phone</span><span class="sxs-lookup"><span data-stu-id="871d7-147">phone</span></span>|<span data-ttu-id="871d7-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="871d7-148">String</span></span>|<span data-ttu-id="871d7-149">O número de telefone para a empresa.</span><span class="sxs-lookup"><span data-stu-id="871d7-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="871d7-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="871d7-150">schedulingPolicy</span></span>|[<span data-ttu-id="871d7-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="871d7-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="871d7-152">Especifica como reservas podem ser criadas para esta empresa.</span><span class="sxs-lookup"><span data-stu-id="871d7-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="871d7-153">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="871d7-153">webSiteUrl</span></span>|<span data-ttu-id="871d7-154">String</span><span class="sxs-lookup"><span data-stu-id="871d7-154">String</span></span>|<span data-ttu-id="871d7-155">A URL do site da web de negócios.</span><span class="sxs-lookup"><span data-stu-id="871d7-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="871d7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="871d7-156">Response</span></span>
<span data-ttu-id="871d7-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="871d7-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="871d7-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="871d7-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="871d7-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="871d7-160">Request</span></span>
<span data-ttu-id="871d7-161">O exemplo a seguir atualiza o endereço de email comercial e o agendamento de política, para alterar o intervalo de tempo de reserva de padrão de negócios para uma hora e Avançar reserva até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="871d7-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="871d7-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="871d7-162">Response</span></span>
<span data-ttu-id="871d7-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="871d7-163">The following is an example of the response.</span></span> <span data-ttu-id="871d7-164">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="871d7-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="871d7-165">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="871d7-165">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
