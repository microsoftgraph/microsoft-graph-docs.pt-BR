---
title: Atualizar bookingservice
description: Atualize as propriedades de um objeto de bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519714"
---
# <a name="update-bookingservice"></a><span data-ttu-id="ae19e-103">Atualizar bookingservice</span><span class="sxs-lookup"><span data-stu-id="ae19e-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae19e-104">Atualize as propriedades de um objeto de [bookingService](../resources/bookingservice.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="ae19e-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="ae19e-105">Eis alguns exemplos que você pode personalizar para um serviço:</span><span class="sxs-lookup"><span data-stu-id="ae19e-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="ae19e-106">Price</span><span class="sxs-lookup"><span data-stu-id="ae19e-106">Price</span></span>
- <span data-ttu-id="ae19e-107">Comprimento típico de um compromisso</span><span class="sxs-lookup"><span data-stu-id="ae19e-107">Typical length of an appointment</span></span>
- <span data-ttu-id="ae19e-108">Reminders</span><span class="sxs-lookup"><span data-stu-id="ae19e-108">Reminders</span></span>
- <span data-ttu-id="ae19e-109">Buffer para definir antes ou término após o serviço a qualquer momento</span><span class="sxs-lookup"><span data-stu-id="ae19e-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="ae19e-110">Parâmetros de [política de agendamento](../resources/bookingschedulingpolicy.md) , como mínimo de aviso do livro ou Cancelar, e se os clientes podem selecionar membros de equipe específico para um compromisso.</span><span class="sxs-lookup"><span data-stu-id="ae19e-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae19e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae19e-111">Permissions</span></span>
<span data-ttu-id="ae19e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae19e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae19e-114">Permission type</span></span>      | <span data-ttu-id="ae19e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae19e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae19e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae19e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="ae19e-117">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ae19e-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ae19e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae19e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae19e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae19e-119">Not supported.</span></span>   |
|<span data-ttu-id="ae19e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae19e-120">Application</span></span> | <span data-ttu-id="ae19e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae19e-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ae19e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae19e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ae19e-123">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ae19e-123">Optional request headers</span></span>
| <span data-ttu-id="ae19e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ae19e-124">Name</span></span>       | <span data-ttu-id="ae19e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae19e-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ae19e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae19e-126">Authorization</span></span>  | <span data-ttu-id="ae19e-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ae19e-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae19e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae19e-128">Request body</span></span>
<span data-ttu-id="ae19e-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ae19e-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ae19e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae19e-132">Property</span></span>     | <span data-ttu-id="ae19e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae19e-133">Type</span></span>   |<span data-ttu-id="ae19e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae19e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae19e-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="ae19e-135">defaultDuration</span></span>|<span data-ttu-id="ae19e-136">Duration</span><span class="sxs-lookup"><span data-stu-id="ae19e-136">Duration</span></span>|<span data-ttu-id="ae19e-137">O comprimento padrão do serviço, representado em número de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="ae19e-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="ae19e-138">Por exemplo, P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="ae19e-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="ae19e-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="ae19e-139">defaultLocation</span></span>|[<span data-ttu-id="ae19e-140">location</span><span class="sxs-lookup"><span data-stu-id="ae19e-140">location</span></span>](../resources/location.md)|<span data-ttu-id="ae19e-141">A localização física padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="ae19e-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="ae19e-142">defaultPrice</span></span>|<span data-ttu-id="ae19e-143">Duplo</span><span class="sxs-lookup"><span data-stu-id="ae19e-143">Double</span></span>|<span data-ttu-id="ae19e-144">O preço monetários padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="ae19e-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="ae19e-145">defaultPriceType</span></span>|<span data-ttu-id="ae19e-146">string</span><span class="sxs-lookup"><span data-stu-id="ae19e-146">string</span></span>|<span data-ttu-id="ae19e-147">A maneira padrão de serviço é cobrada.</span><span class="sxs-lookup"><span data-stu-id="ae19e-147">The default way the service is charged.</span></span> <span data-ttu-id="ae19e-148">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ae19e-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="ae19e-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="ae19e-149">defaultReminders</span></span>|<span data-ttu-id="ae19e-150">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="ae19e-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="ae19e-151">O padrão é definido de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="ae19e-152">O valor dessa propriedade está disponível somente quando a ler este **bookingService** pela sua identificação.</span><span class="sxs-lookup"><span data-stu-id="ae19e-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="ae19e-153">description</span><span class="sxs-lookup"><span data-stu-id="ae19e-153">description</span></span>|<span data-ttu-id="ae19e-154">String</span><span class="sxs-lookup"><span data-stu-id="ae19e-154">String</span></span>|<span data-ttu-id="ae19e-155">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-155">A text description for the service.</span></span>|
|<span data-ttu-id="ae19e-156">displayName</span><span class="sxs-lookup"><span data-stu-id="ae19e-156">displayName</span></span>|<span data-ttu-id="ae19e-157">String</span><span class="sxs-lookup"><span data-stu-id="ae19e-157">String</span></span>|<span data-ttu-id="ae19e-158">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-158">A service name.</span></span>|
|<span data-ttu-id="ae19e-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ae19e-159">emailAddress</span></span>|<span data-ttu-id="ae19e-160">String</span><span class="sxs-lookup"><span data-stu-id="ae19e-160">String</span></span>|<span data-ttu-id="ae19e-161">Um email:  </span><span class="sxs-lookup"><span data-stu-id="ae19e-161">An email address</span></span>|
|<span data-ttu-id="ae19e-162">id</span><span class="sxs-lookup"><span data-stu-id="ae19e-162">id</span></span>|<span data-ttu-id="ae19e-163">String</span><span class="sxs-lookup"><span data-stu-id="ae19e-163">String</span></span>| <span data-ttu-id="ae19e-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae19e-164">Read-only.</span></span>|
|<span data-ttu-id="ae19e-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="ae19e-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="ae19e-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae19e-166">Boolean</span></span>|<span data-ttu-id="ae19e-167">True significa que esse serviço não está disponível para os clientes de reserva.</span><span class="sxs-lookup"><span data-stu-id="ae19e-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="ae19e-168">Observações</span><span class="sxs-lookup"><span data-stu-id="ae19e-168">notes</span></span>|<span data-ttu-id="ae19e-169">String</span><span class="sxs-lookup"><span data-stu-id="ae19e-169">String</span></span>|<span data-ttu-id="ae19e-170">Informações adicionais sobre esse serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-170">Additional information about this service.</span></span>|
|<span data-ttu-id="ae19e-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="ae19e-171">postBuffer</span></span>|<span data-ttu-id="ae19e-172">Duration</span><span class="sxs-lookup"><span data-stu-id="ae19e-172">Duration</span></span>|<span data-ttu-id="ae19e-173">Encerra o tempo de buffer após um compromisso para este serviço e antes que a próxima compromisso do cliente pode ser agendado.</span><span class="sxs-lookup"><span data-stu-id="ae19e-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="ae19e-174">preBuffer</span><span class="sxs-lookup"><span data-stu-id="ae19e-174">preBuffer</span></span>|<span data-ttu-id="ae19e-175">Duration</span><span class="sxs-lookup"><span data-stu-id="ae19e-175">Duration</span></span>|<span data-ttu-id="ae19e-176">O tempo de buffer antes de um compromisso para esse serviço pode iniciar.</span><span class="sxs-lookup"><span data-stu-id="ae19e-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="ae19e-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="ae19e-177">schedulingPolicy</span></span>|[<span data-ttu-id="ae19e-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="ae19e-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="ae19e-179">O conjunto de diretivas que determinam como compromissos para esse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ae19e-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="ae19e-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="ae19e-180">staffMemberIds</span></span>|<span data-ttu-id="ae19e-181">String collection</span><span class="sxs-lookup"><span data-stu-id="ae19e-181">String collection</span></span>|<span data-ttu-id="ae19e-182">Representa os [membros da equipe](../resources/bookingstaffmember.md) que forneça esse serviço.</span><span class="sxs-lookup"><span data-stu-id="ae19e-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="ae19e-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae19e-183">Response</span></span>
<span data-ttu-id="ae19e-p106">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae19e-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae19e-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae19e-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae19e-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae19e-187">Request</span></span>
<span data-ttu-id="ae19e-188">O exemplo a seguir atualiza a duração do serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="ae19e-188">The following example updates the duration of the specified service.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a><span data-ttu-id="ae19e-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae19e-189">Response</span></span>
<span data-ttu-id="ae19e-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae19e-190">The following is an example of the response.</span></span>
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
