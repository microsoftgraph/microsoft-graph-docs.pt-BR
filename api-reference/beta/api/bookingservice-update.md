---
title: Atualizar bookingservice
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: e39ad73b7f9acf2337db517e67895bc4601598a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035348"
---
# <a name="update-bookingservice"></a><span data-ttu-id="141f1-104">Atualizar bookingservice</span><span class="sxs-lookup"><span data-stu-id="141f1-104">Update bookingservice</span></span>

 > <span data-ttu-id="141f1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="141f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="141f1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="141f1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="141f1-107">Atualize as propriedades de um objeto de [bookingService](../resources/bookingservice.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="141f1-107">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="141f1-108">Eis alguns exemplos que você pode personalizar para um serviço:</span><span class="sxs-lookup"><span data-stu-id="141f1-108">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="141f1-109">Price</span><span class="sxs-lookup"><span data-stu-id="141f1-109">Price</span></span>
- <span data-ttu-id="141f1-110">Comprimento típico de um compromisso</span><span class="sxs-lookup"><span data-stu-id="141f1-110">Typical length of an appointment</span></span>
- <span data-ttu-id="141f1-111">Reminders</span><span class="sxs-lookup"><span data-stu-id="141f1-111">Reminders</span></span>
- <span data-ttu-id="141f1-112">Buffer para definir antes ou término após o serviço a qualquer momento</span><span class="sxs-lookup"><span data-stu-id="141f1-112">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="141f1-113">Parâmetros de [política de agendamento](../resources/bookingschedulingpolicy.md) , como mínimo de aviso do livro ou Cancelar, e se os clientes podem selecionar membros de equipe específico para um compromisso.</span><span class="sxs-lookup"><span data-stu-id="141f1-113">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="141f1-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="141f1-114">Permissions</span></span>
<span data-ttu-id="141f1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="141f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="141f1-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="141f1-117">Permission type</span></span>      | <span data-ttu-id="141f1-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="141f1-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="141f1-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="141f1-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="141f1-120">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="141f1-120">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="141f1-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="141f1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="141f1-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="141f1-122">Not supported.</span></span>   |
|<span data-ttu-id="141f1-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="141f1-123">Application</span></span> | <span data-ttu-id="141f1-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="141f1-124">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="141f1-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="141f1-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="141f1-126">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="141f1-126">Optional request headers</span></span>
| <span data-ttu-id="141f1-127">Nome</span><span class="sxs-lookup"><span data-stu-id="141f1-127">Name</span></span>       | <span data-ttu-id="141f1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="141f1-128">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="141f1-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="141f1-129">Authorization</span></span>  | <span data-ttu-id="141f1-130">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="141f1-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="141f1-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="141f1-131">Request body</span></span>
<span data-ttu-id="141f1-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="141f1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="141f1-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="141f1-135">Property</span></span>     | <span data-ttu-id="141f1-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="141f1-136">Type</span></span>   |<span data-ttu-id="141f1-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="141f1-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="141f1-138">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="141f1-138">defaultDuration</span></span>|<span data-ttu-id="141f1-139">Duração</span><span class="sxs-lookup"><span data-stu-id="141f1-139">Duration</span></span>|<span data-ttu-id="141f1-140">O comprimento padrão do serviço, representado em número de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="141f1-140">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="141f1-141">Por exemplo, P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="141f1-141">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="141f1-142">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="141f1-142">defaultLocation</span></span>|[<span data-ttu-id="141f1-143">location</span><span class="sxs-lookup"><span data-stu-id="141f1-143">location</span></span>](../resources/location.md)|<span data-ttu-id="141f1-144">A localização física padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-144">The default physical location for the service.</span></span>|
|<span data-ttu-id="141f1-145">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="141f1-145">defaultPrice</span></span>|<span data-ttu-id="141f1-146">Duplo</span><span class="sxs-lookup"><span data-stu-id="141f1-146">Double</span></span>|<span data-ttu-id="141f1-147">O preço monetários padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-147">The default monetary price for the service.</span></span>|
|<span data-ttu-id="141f1-148">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="141f1-148">defaultPriceType</span></span>|<span data-ttu-id="141f1-149">string</span><span class="sxs-lookup"><span data-stu-id="141f1-149">string</span></span>|<span data-ttu-id="141f1-150">A maneira padrão de serviço é cobrada.</span><span class="sxs-lookup"><span data-stu-id="141f1-150">The default way the service is charged.</span></span> <span data-ttu-id="141f1-151">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="141f1-151">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="141f1-152">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="141f1-152">defaultReminders</span></span>|<span data-ttu-id="141f1-153">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="141f1-153">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="141f1-154">O padrão é definido de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-154">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="141f1-155">O valor dessa propriedade está disponível somente quando a ler este **bookingService** pela sua identificação.</span><span class="sxs-lookup"><span data-stu-id="141f1-155">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="141f1-156">description</span><span class="sxs-lookup"><span data-stu-id="141f1-156">description</span></span>|<span data-ttu-id="141f1-157">String</span><span class="sxs-lookup"><span data-stu-id="141f1-157">String</span></span>|<span data-ttu-id="141f1-158">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-158">A text description for the service.</span></span>|
|<span data-ttu-id="141f1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="141f1-159">displayName</span></span>|<span data-ttu-id="141f1-160">String</span><span class="sxs-lookup"><span data-stu-id="141f1-160">String</span></span>|<span data-ttu-id="141f1-161">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-161">A service name.</span></span>|
|<span data-ttu-id="141f1-162">emailAddress</span><span class="sxs-lookup"><span data-stu-id="141f1-162">emailAddress</span></span>|<span data-ttu-id="141f1-163">String</span><span class="sxs-lookup"><span data-stu-id="141f1-163">String</span></span>|<span data-ttu-id="141f1-164">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="141f1-164">An email address</span></span>|
|<span data-ttu-id="141f1-165">id</span><span class="sxs-lookup"><span data-stu-id="141f1-165">id</span></span>|<span data-ttu-id="141f1-166">String</span><span class="sxs-lookup"><span data-stu-id="141f1-166">String</span></span>| <span data-ttu-id="141f1-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="141f1-167">Read-only.</span></span>|
|<span data-ttu-id="141f1-168">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="141f1-168">isHiddenFromCustomers</span></span>|<span data-ttu-id="141f1-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="141f1-169">Boolean</span></span>|<span data-ttu-id="141f1-170">True significa que esse serviço não está disponível para os clientes de reserva.</span><span class="sxs-lookup"><span data-stu-id="141f1-170">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="141f1-171">Observações</span><span class="sxs-lookup"><span data-stu-id="141f1-171">notes</span></span>|<span data-ttu-id="141f1-172">String</span><span class="sxs-lookup"><span data-stu-id="141f1-172">String</span></span>|<span data-ttu-id="141f1-173">Informações adicionais sobre esse serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-173">Additional information about this service.</span></span>|
|<span data-ttu-id="141f1-174">postBuffer</span><span class="sxs-lookup"><span data-stu-id="141f1-174">postBuffer</span></span>|<span data-ttu-id="141f1-175">Duração</span><span class="sxs-lookup"><span data-stu-id="141f1-175">Duration</span></span>|<span data-ttu-id="141f1-176">Encerra o tempo de buffer após um compromisso para este serviço e antes que a próxima compromisso do cliente pode ser agendado.</span><span class="sxs-lookup"><span data-stu-id="141f1-176">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="141f1-177">preBuffer</span><span class="sxs-lookup"><span data-stu-id="141f1-177">preBuffer</span></span>|<span data-ttu-id="141f1-178">Duração</span><span class="sxs-lookup"><span data-stu-id="141f1-178">Duration</span></span>|<span data-ttu-id="141f1-179">O tempo de buffer antes de um compromisso para esse serviço pode iniciar.</span><span class="sxs-lookup"><span data-stu-id="141f1-179">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="141f1-180">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="141f1-180">schedulingPolicy</span></span>|[<span data-ttu-id="141f1-181">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="141f1-181">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="141f1-182">O conjunto de diretivas que determinam como compromissos para esse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="141f1-182">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="141f1-183">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="141f1-183">staffMemberIds</span></span>|<span data-ttu-id="141f1-184">String collection</span><span class="sxs-lookup"><span data-stu-id="141f1-184">String collection</span></span>|<span data-ttu-id="141f1-185">Representa os [membros da equipe](../resources/bookingstaffmember.md) que forneça esse serviço.</span><span class="sxs-lookup"><span data-stu-id="141f1-185">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="141f1-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="141f1-186">Response</span></span>
<span data-ttu-id="141f1-p108">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="141f1-p108">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="141f1-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="141f1-189">Example</span></span>
##### <a name="request"></a><span data-ttu-id="141f1-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="141f1-190">Request</span></span>
<span data-ttu-id="141f1-191">O exemplo a seguir atualiza a duração do serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="141f1-191">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="141f1-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="141f1-192">Response</span></span>
<span data-ttu-id="141f1-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="141f1-193">The following is an example of the response.</span></span> 
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->