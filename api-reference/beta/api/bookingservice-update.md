---
title: Atualizar bookingservice
description: Atualiza as propriedades de um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461630"
---
# <a name="update-bookingservice"></a><span data-ttu-id="5dc8a-103">Atualizar bookingservice</span><span class="sxs-lookup"><span data-stu-id="5dc8a-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc8a-104">Atualiza as propriedades de um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="5dc8a-105">Veja a seguir alguns exemplos que você pode personalizar para um serviço:</span><span class="sxs-lookup"><span data-stu-id="5dc8a-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="5dc8a-106">Price</span><span class="sxs-lookup"><span data-stu-id="5dc8a-106">Price</span></span>
- <span data-ttu-id="5dc8a-107">Tamanho típico de um compromisso</span><span class="sxs-lookup"><span data-stu-id="5dc8a-107">Typical length of an appointment</span></span>
- <span data-ttu-id="5dc8a-108">Lembretes</span><span class="sxs-lookup"><span data-stu-id="5dc8a-108">Reminders</span></span>
- <span data-ttu-id="5dc8a-109">Qualquer buffer de tempo a ser configurado antes ou termine após o serviço</span><span class="sxs-lookup"><span data-stu-id="5dc8a-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="5dc8a-110">Parâmetros de [política de agendamento](../resources/bookingschedulingpolicy.md) , como o aviso mínimo, para livro ou cancelamento, e se os clientes podem selecionar membros específicos da equipe para um compromisso.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc8a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dc8a-111">Permissions</span></span>
<span data-ttu-id="5dc8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc8a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc8a-114">Permission type</span></span>      | <span data-ttu-id="5dc8a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dc8a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dc8a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc8a-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="5dc8a-117">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="5dc8a-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5dc8a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc8a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc8a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-119">Not supported.</span></span>   |
|<span data-ttu-id="5dc8a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc8a-120">Application</span></span> | <span data-ttu-id="5dc8a-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5dc8a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc8a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5dc8a-123">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5dc8a-123">Optional request headers</span></span>
| <span data-ttu-id="5dc8a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5dc8a-124">Name</span></span>       | <span data-ttu-id="5dc8a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc8a-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5dc8a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dc8a-126">Authorization</span></span>  | <span data-ttu-id="5dc8a-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5dc8a-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc8a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc8a-128">Request body</span></span>
<span data-ttu-id="5dc8a-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5dc8a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dc8a-132">Property</span></span>     | <span data-ttu-id="5dc8a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc8a-133">Type</span></span>   |<span data-ttu-id="5dc8a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc8a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dc8a-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="5dc8a-135">defaultDuration</span></span>|<span data-ttu-id="5dc8a-136">Duração</span><span class="sxs-lookup"><span data-stu-id="5dc8a-136">Duration</span></span>|<span data-ttu-id="5dc8a-137">O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="5dc8a-138">Por exemplo, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="5dc8a-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="5dc8a-139">defaultLocation</span></span>|[<span data-ttu-id="5dc8a-140">location</span><span class="sxs-lookup"><span data-stu-id="5dc8a-140">location</span></span>](../resources/location.md)|<span data-ttu-id="5dc8a-141">O local físico padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="5dc8a-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="5dc8a-142">defaultPrice</span></span>|<span data-ttu-id="5dc8a-143">Duplo</span><span class="sxs-lookup"><span data-stu-id="5dc8a-143">Double</span></span>|<span data-ttu-id="5dc8a-144">O preço monetário padrão do serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="5dc8a-145">defaultPricetype</span><span class="sxs-lookup"><span data-stu-id="5dc8a-145">defaultPriceType</span></span>|<span data-ttu-id="5dc8a-146">string</span><span class="sxs-lookup"><span data-stu-id="5dc8a-146">string</span></span>|<span data-ttu-id="5dc8a-147">O modo padrão pelo qual o serviço é cobrado.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-147">The default way the service is charged.</span></span> <span data-ttu-id="5dc8a-148">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="5dc8a-149">defaultLembrers</span><span class="sxs-lookup"><span data-stu-id="5dc8a-149">defaultReminders</span></span>|<span data-ttu-id="5dc8a-150">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="5dc8a-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="5dc8a-151">O conjunto padrão de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="5dc8a-152">O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="5dc8a-153">description</span><span class="sxs-lookup"><span data-stu-id="5dc8a-153">description</span></span>|<span data-ttu-id="5dc8a-154">String</span><span class="sxs-lookup"><span data-stu-id="5dc8a-154">String</span></span>|<span data-ttu-id="5dc8a-155">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-155">A text description for the service.</span></span>|
|<span data-ttu-id="5dc8a-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5dc8a-156">displayName</span></span>|<span data-ttu-id="5dc8a-157">String</span><span class="sxs-lookup"><span data-stu-id="5dc8a-157">String</span></span>|<span data-ttu-id="5dc8a-158">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-158">A service name.</span></span>|
|<span data-ttu-id="5dc8a-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5dc8a-159">emailAddress</span></span>|<span data-ttu-id="5dc8a-160">String</span><span class="sxs-lookup"><span data-stu-id="5dc8a-160">String</span></span>|<span data-ttu-id="5dc8a-161">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="5dc8a-161">An email address</span></span>|
|<span data-ttu-id="5dc8a-162">id</span><span class="sxs-lookup"><span data-stu-id="5dc8a-162">id</span></span>|<span data-ttu-id="5dc8a-163">String</span><span class="sxs-lookup"><span data-stu-id="5dc8a-163">String</span></span>| <span data-ttu-id="5dc8a-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-164">Read-only.</span></span>|
|<span data-ttu-id="5dc8a-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="5dc8a-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="5dc8a-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="5dc8a-166">Boolean</span></span>|<span data-ttu-id="5dc8a-167">True significa que este serviço não está disponível para os clientes para reserva.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="5dc8a-168">notes</span><span class="sxs-lookup"><span data-stu-id="5dc8a-168">notes</span></span>|<span data-ttu-id="5dc8a-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc8a-169">String</span></span>|<span data-ttu-id="5dc8a-170">Informações adicionais sobre este serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-170">Additional information about this service.</span></span>|
|<span data-ttu-id="5dc8a-171">Buffer</span><span class="sxs-lookup"><span data-stu-id="5dc8a-171">postBuffer</span></span>|<span data-ttu-id="5dc8a-172">Duração</span><span class="sxs-lookup"><span data-stu-id="5dc8a-172">Duration</span></span>|<span data-ttu-id="5dc8a-173">O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="5dc8a-174">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="5dc8a-174">preBuffer</span></span>|<span data-ttu-id="5dc8a-175">Duração</span><span class="sxs-lookup"><span data-stu-id="5dc8a-175">Duration</span></span>|<span data-ttu-id="5dc8a-176">O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="5dc8a-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="5dc8a-177">schedulingPolicy</span></span>|[<span data-ttu-id="5dc8a-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="5dc8a-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="5dc8a-179">O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="5dc8a-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="5dc8a-180">staffMemberIds</span></span>|<span data-ttu-id="5dc8a-181">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc8a-181">String collection</span></span>|<span data-ttu-id="5dc8a-182">Representa os [membros da equipe](../resources/bookingstaffmember.md) que fornecem esse serviço.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="5dc8a-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc8a-183">Response</span></span>
<span data-ttu-id="5dc8a-p106">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5dc8a-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc8a-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dc8a-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc8a-187">Request</span></span>
<span data-ttu-id="5dc8a-188">O exemplo a seguir atualiza a duração do serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-188">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5dc8a-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc8a-189">Response</span></span>
<span data-ttu-id="5dc8a-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc8a-190">The following is an example of the response.</span></span>
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
