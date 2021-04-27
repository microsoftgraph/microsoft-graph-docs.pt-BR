---
title: 'user: findMeetingTimes'
description: Localize as sugestões de hora da reunião com base no organizador e na disponibilidade dos participantes, assim como nas restrições de horário ou local especificadas como parâmetros.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9fbb914533b8eedce9e896a86886bdba656d6034
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052653"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="97fae-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="97fae-103">user: findMeetingTimes</span></span>

<span data-ttu-id="97fae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97fae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97fae-105">Localize as sugestões de hora da reunião com base no organizador e na disponibilidade dos participantes, assim como nas restrições de horário ou local especificadas como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="97fae-105">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="97fae-p101">Se **findMeetingTimes** não retorna nenhuma sugestão de reunião, a resposta seria indicar um motivo na propriedade **emptySuggestionsReason**. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.</span><span class="sxs-lookup"><span data-stu-id="97fae-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

<span data-ttu-id="97fae-108">O algoritmo usado para ilustrar horários de reunião e locais passa por ajuste fino de tempos em tempos.</span><span class="sxs-lookup"><span data-stu-id="97fae-108">The algorithm used to suggest meeting times and locations undergoes fine-tuning from time to time.</span></span> <span data-ttu-id="97fae-109">Cenários como ambientes de teste onde permanecem estáticos parâmetros de entrada e dados de calendário, espere que os resultados sugeridos sejam diferentes ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="97fae-109">In scenarios like test environments where the input parameters and calendar data remain static, expect that the suggested results may differ over time.</span></span>


## <a name="permissions"></a><span data-ttu-id="97fae-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="97fae-110">Permissions</span></span>
<span data-ttu-id="97fae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97fae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97fae-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97fae-113">Permission type</span></span>      | <span data-ttu-id="97fae-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97fae-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97fae-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97fae-115">Delegated (work or school account)</span></span> | <span data-ttu-id="97fae-116">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="97fae-116">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="97fae-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97fae-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97fae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97fae-118">Not supported.</span></span>    |
|<span data-ttu-id="97fae-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97fae-119">Application</span></span> | <span data-ttu-id="97fae-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97fae-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97fae-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97fae-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="97fae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97fae-122">Request headers</span></span>
| <span data-ttu-id="97fae-123">Nome</span><span class="sxs-lookup"><span data-stu-id="97fae-123">Name</span></span>       | <span data-ttu-id="97fae-124">Valor</span><span class="sxs-lookup"><span data-stu-id="97fae-124">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97fae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="97fae-125">Authorization</span></span>  | <span data-ttu-id="97fae-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97fae-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97fae-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="97fae-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="97fae-p105">Uma cadeia de caracteres que representa um fuso horário específico para a resposta; por exemplo, "Hora Oficial do Pacífico". Opcional. UTC será usado se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="97fae-p105">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97fae-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97fae-132">Request body</span></span>
<span data-ttu-id="97fae-p106">Todos os parâmetros suportados estão listados abaixo. Dependendo do cenário, especifique um objeto JSON para cada um dos parâmetros necessários no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97fae-p106">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="97fae-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="97fae-135">Parameter</span></span>    | <span data-ttu-id="97fae-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="97fae-136">Type</span></span>   |<span data-ttu-id="97fae-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="97fae-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97fae-138">attendees</span><span class="sxs-lookup"><span data-stu-id="97fae-138">attendees</span></span>|<span data-ttu-id="97fae-139">Coleção [attendeeBase](../resources/attendeebase.md)</span><span class="sxs-lookup"><span data-stu-id="97fae-139">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="97fae-140">Uma coleção de participantes ou recursos da reunião.</span><span class="sxs-lookup"><span data-stu-id="97fae-140">A collection of attendees or resources for the meeting.</span></span> <span data-ttu-id="97fae-141">Na propriedade **tipo correspondente,** especifique `required` ou para uma pessoa e para um recurso como sala de `optional` `resource` reunião.</span><span class="sxs-lookup"><span data-stu-id="97fae-141">In the corresponding **type** property, specify `required` or `optional` for a person and `resource` for a resource like meeting room.</span></span> <span data-ttu-id="97fae-142">Se não for especificado, **findMeetingTimes** assume `required` a propriedade **type.**</span><span class="sxs-lookup"><span data-stu-id="97fae-142">If not specified, **findMeetingTimes** assumes `required` for the **type** property.</span></span> <span data-ttu-id="97fae-143">Uma coleção vazia faz com que **findMeetingTimes** procure gratuitamente alocações de tempo somente para o organizador.</span><span class="sxs-lookup"><span data-stu-id="97fae-143">An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer.</span></span> <span data-ttu-id="97fae-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-144">Optional.</span></span>|
|<span data-ttu-id="97fae-145">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="97fae-145">isOrganizerOptional</span></span>|<span data-ttu-id="97fae-146">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="97fae-146">Edm.Boolean</span></span>|<span data-ttu-id="97fae-p108">Especifique `True` se o organizador não tiver necessariamente que participar. O padrão é `false`. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-p108">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="97fae-150">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="97fae-150">locationConstraint</span></span>|[<span data-ttu-id="97fae-151">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="97fae-151">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="97fae-p109">Os requisitos do organizador sobre o local da reunião, tal como se é necessário sugerir de um local de encontro, ou há locais específicos apenas onde a reunião pode ocorrer. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-p109">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="97fae-154">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="97fae-154">maxCandidates</span></span>|<span data-ttu-id="97fae-155">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="97fae-155">Edm.Int32</span></span>|<span data-ttu-id="97fae-p110">O número máximo de sugestões de horários de reunião a ser retornados. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-p110">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="97fae-158">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="97fae-158">meetingDuration</span></span>|<span data-ttu-id="97fae-159">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="97fae-159">Edm.Duration</span></span>|<span data-ttu-id="97fae-160">O tamanho da reunião, denotado no [formato ISO 8601.](https://www.iso.org/iso/iso8601)</span><span class="sxs-lookup"><span data-stu-id="97fae-160">The length of the meeting, denoted in [ISO 8601](https://www.iso.org/iso/iso8601) format.</span></span> <span data-ttu-id="97fae-161">Por exemplo, 1 hora é denotada como 'PT1H', onde 'P' é o designador de duração, 'T' é o designador de hora e 'H' é o designador de hora.</span><span class="sxs-lookup"><span data-stu-id="97fae-161">For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator.</span></span> <span data-ttu-id="97fae-162">Use M para indicar minutos para a duração; por exemplo, 2 horas e 30 minutos seria 'PT2H30M'.</span><span class="sxs-lookup"><span data-stu-id="97fae-162">Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'.</span></span> <span data-ttu-id="97fae-163">Se a duração da reunião não for especificada, **findMeetingTimes** usará o padrão de 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="97fae-163">If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes.</span></span> <span data-ttu-id="97fae-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-164">Optional.</span></span>|
|<span data-ttu-id="97fae-165">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="97fae-165">minimumAttendeePercentage</span></span>|<span data-ttu-id="97fae-166">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="97fae-166">Edm.Double</span></span>| <span data-ttu-id="97fae-p112">O mínimo necessário de [confiança](#the-confidence-of-a-meeting-suggestion) para um intervalo de tempo a ser retornado na resposta. É um valor de % variando de 0 a 100. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-p112">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="97fae-170">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="97fae-170">returnSuggestionReasons</span></span>|<span data-ttu-id="97fae-171">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="97fae-171">Edm.Boolean</span></span>|<span data-ttu-id="97fae-p113">Especifique `True` para retornar um motivo para cada sugestão de reunião na propriedade **suggestionReason**. O padrão é `false` para não retornar essa propriedade. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-p113">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="97fae-175">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="97fae-175">timeConstraint</span></span>|[<span data-ttu-id="97fae-176">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="97fae-176">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="97fae-p114">Qualquer restrição de tempo para uma reunião, o que pode incluir a natureza da reunião (propriedade **activityDomain**) e possíveis intervalos de tempo da reunião (propriedade **timeSlots**). **findMeetingTimes** pressupõe **activityDomain** como `work` se você não especificar este parâmetro. Opcional.</span><span class="sxs-lookup"><span data-stu-id="97fae-p114">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="97fae-180">A tabela a seguir descreve as restrições que você pode especificar ainda mais no parâmetro **timeConstraint**.</span><span class="sxs-lookup"><span data-stu-id="97fae-180">The following table describes the restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="97fae-181">valor activityDomain em timeConstraint</span><span class="sxs-lookup"><span data-stu-id="97fae-181">activityDomain value in timeConstraint</span></span>|<span data-ttu-id="97fae-182">Sugestões de horário para reuniões</span><span class="sxs-lookup"><span data-stu-id="97fae-182">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="97fae-183">trabalho</span><span class="sxs-lookup"><span data-stu-id="97fae-183">work</span></span>| <span data-ttu-id="97fae-p115">As sugestões são nas horas de trabalho do usuário que são definidas na configuração do calendário do usuário e podem ser personalizadas pelo usuário ou administrador. As horas de trabalho padrão são de segunda a sexta, das 8h às 17h, no fuso horário definido para a caixa de correio. Este é o valor padrão se nenhum **activityDomain** for especificado.</span><span class="sxs-lookup"><span data-stu-id="97fae-p115">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="97fae-187">pessoal</span><span class="sxs-lookup"><span data-stu-id="97fae-187">personal</span></span>| <span data-ttu-id="97fae-p116">As sugestões são dentro das horas de trabalho do usuário, e sábado e domingo. O padrão é de segunda a sexta, das 8h às 17h, na configuração de fuso horário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="97fae-p116">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="97fae-190">irrestrito</span><span class="sxs-lookup"><span data-stu-id="97fae-190">unrestricted</span></span> | <span data-ttu-id="97fae-191">As sugestões podem ser todas as horas do dia, todos os dias da semana.</span><span class="sxs-lookup"><span data-stu-id="97fae-191">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="97fae-192">desconhecido</span><span class="sxs-lookup"><span data-stu-id="97fae-192">unknown</span></span> | <span data-ttu-id="97fae-p117">Não use esse valor, uma vez que ele será substituído no futuro. Atualmente, se comporta da mesma forma que o `work`. Altere qualquer código existente para usar o `work`, `personal` ou `unrestricted` conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="97fae-p117">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>|


<span data-ttu-id="97fae-p118">Com base nos parâmetros especificados,**findMeetingTimes** verifica o status disponível/ocupado nos calendários principais do organizador e dos participantes. A ação calcula os melhores possíveis horários de reuniões e retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="97fae-p118">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="97fae-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="97fae-198">Response</span></span>

<span data-ttu-id="97fae-199">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97fae-199">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="97fae-p119">Um **meetingTimeSuggestionsResult** inclui uma coleção de sugestões de reunião e uma propriedade **emptySuggestionsReason**. Cada sugestão é definida como uma [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), e participantes com um nível de confiança de 50% na média para participar ou uma % específica que definida no parâmetro **minimumAttendeePercentage**.</span><span class="sxs-lookup"><span data-stu-id="97fae-p119">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="97fae-202">Por padrão, cada sugestão de horário de reunião é retornado em UTC.</span><span class="sxs-lookup"><span data-stu-id="97fae-202">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="97fae-p120">Se **findMeetingTimes** não retorna nenhuma sugestão de reunião, a resposta seria indicar um motivo na propriedade **emptySuggestionsReason**. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.</span><span class="sxs-lookup"><span data-stu-id="97fae-p120">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="97fae-205">A confiança de uma sugestão de reunião</span><span class="sxs-lookup"><span data-stu-id="97fae-205">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="97fae-206">A propriedade **confidence** de uma **meetingTimeSuggestion** varia de 0% a 100% e representa a chance de que todos os participantes compareçam à reunião, com base em seu status disponível/ocupado:</span><span class="sxs-lookup"><span data-stu-id="97fae-206">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="97fae-207">Para cada participante, um status livre para um período de tempo de reunião especificado corresponde à chance de 100% de presença, status desconhecido 49% e status ocupado 0%.</span><span class="sxs-lookup"><span data-stu-id="97fae-207">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="97fae-208">A confiança na sugestão de um horário de reunião é calculada pela média da chance de presença de todos os participantes especificados para essa reunião.</span><span class="sxs-lookup"><span data-stu-id="97fae-208">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="97fae-p121">Se houver diversas sugestões de horário de reunião, a ação **findMeetingTimes** primeiramente classifica as sugestões por seu valor de confiança computado que vai de alto para baixo. Se houver sugestões com a mesma confiança, a ação ordena essas sugestões em ordem cronológica.</span><span class="sxs-lookup"><span data-stu-id="97fae-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>
- <span data-ttu-id="97fae-p122">Você pode usar o parâmetro opcional **minimumAttendeePercentage** **findMeetingTimes** para especificar que apenas as sugestões de horário da reunião com pelo menos determinado nível de confiança retornem. Por exemplo, você pode especificar uma **minimumAttendeePercentage** de 80% se você quiser apenas sugestões que tenham uma chance de 80% ou mais de que todos os participantes comparecerão. Se você não especificar **minimumAttendeePercentage**, **findMeetingTimes** pressupõe um valor de 50%.</span><span class="sxs-lookup"><span data-stu-id="97fae-p122">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>

<span data-ttu-id="97fae-214">Por exemplo, se uma sugestão de horário de reunião envolve três participantes com o seguinte status livre/ocupado:</span><span class="sxs-lookup"><span data-stu-id="97fae-214">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="97fae-215">**Participante**</span><span class="sxs-lookup"><span data-stu-id="97fae-215">**Attendee**</span></span>|<span data-ttu-id="97fae-216">**Status disponível/ocupado**</span><span class="sxs-lookup"><span data-stu-id="97fae-216">**Free/busy status**</span></span>|<span data-ttu-id="97fae-217">**% de chance de comparecer**</span><span class="sxs-lookup"><span data-stu-id="97fae-217">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="97fae-218">Sara</span><span class="sxs-lookup"><span data-stu-id="97fae-218">Dana</span></span> | <span data-ttu-id="97fae-219">Disponível</span><span class="sxs-lookup"><span data-stu-id="97fae-219">Free</span></span> | <span data-ttu-id="97fae-220">100%</span><span class="sxs-lookup"><span data-stu-id="97fae-220">100%</span></span> |
|<span data-ttu-id="97fae-221">Davi</span><span class="sxs-lookup"><span data-stu-id="97fae-221">John</span></span> | <span data-ttu-id="97fae-222">Desconhecido</span><span class="sxs-lookup"><span data-stu-id="97fae-222">Unknown</span></span> | <span data-ttu-id="97fae-223">49%</span><span class="sxs-lookup"><span data-stu-id="97fae-223">49%</span></span> |
|<span data-ttu-id="97fae-224">Sara</span><span class="sxs-lookup"><span data-stu-id="97fae-224">Samantha</span></span> | <span data-ttu-id="97fae-225">Ocupado</span><span class="sxs-lookup"><span data-stu-id="97fae-225">Busy</span></span> | <span data-ttu-id="97fae-226">0%</span><span class="sxs-lookup"><span data-stu-id="97fae-226">0%</span></span> |

<span data-ttu-id="97fae-227">Então a confiança na sugestão do horário da reunião, que corresponde à chance média de presença, é (100% + 49% + 0%) /3 = 49.66%.</span><span class="sxs-lookup"><span data-stu-id="97fae-227">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="97fae-228">Se você especificar um **minimumAttendeePercentage** de 80% em uma operação **findMeetingTimes**, pois 49,66%< 80%, a operação não sugerirá esse horário na resposta.</span><span class="sxs-lookup"><span data-stu-id="97fae-228">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="97fae-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97fae-229">Example</span></span>

<span data-ttu-id="97fae-230">O exemplo a seguir mostra como encontrar um horário para reunir-se em um local predeterminado e solicitar um motivo para cada sugestão, especificando os seguintes parâmetros no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="97fae-230">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="97fae-231">**attendees**</span><span class="sxs-lookup"><span data-stu-id="97fae-231">**attendees**</span></span>
- <span data-ttu-id="97fae-232">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="97fae-232">**locationConstraint**</span></span>
- <span data-ttu-id="97fae-233">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="97fae-233">**timeConstraint**</span></span>
- <span data-ttu-id="97fae-234">**isOrganizerOptional**</span><span class="sxs-lookup"><span data-stu-id="97fae-234">**isOrganizerOptional**</span></span>
- <span data-ttu-id="97fae-235">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="97fae-235">**meetingDuration**</span></span>
- <span data-ttu-id="97fae-236">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="97fae-236">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="97fae-237">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="97fae-237">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="97fae-238">Definindo o parâmetro **returnSuggestionReasons**, você também obtém uma explicação na propriedade **suggestionReason** para cada sugestão, se **findMeetingTimes** retornar qualquer sugestão.</span><span class="sxs-lookup"><span data-stu-id="97fae-238">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="97fae-239">Observe que a solicitação especifica o tempo no fuso horário PST.</span><span class="sxs-lookup"><span data-stu-id="97fae-239">Notice that the request specifies time in the PST time zone.</span></span> <span data-ttu-id="97fae-240">Por padrão, a resposta retorna horário em sugestões UTC.</span><span class="sxs-lookup"><span data-stu-id="97fae-240">By default, the response returns meeting time suggestions in UTC.</span></span> <span data-ttu-id="97fae-241">Você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar os valores de horário para o Horário Padrão do Pacífico na resposta.</span><span class="sxs-lookup"><span data-stu-id="97fae-241">You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="97fae-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97fae-242">Request</span></span>
<span data-ttu-id="97fae-243">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="97fae-243">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97fae-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="97fae-244">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/beta/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Alex Wilbur",
        "address": "alexw@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeSlots": [ 
      { 
        "start": { 
          "dateTime": "2019-04-16T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2019-04-18T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "isOrganizerOptional": "false",
  "meetingDuration": "PT1H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```
# <a name="c"></a>[<span data-ttu-id="97fae-245">C#</span><span class="sxs-lookup"><span data-stu-id="97fae-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-findmeetingtimes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97fae-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97fae-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-findmeetingtimes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97fae-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97fae-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-findmeetingtimes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97fae-248">Java</span><span class="sxs-lookup"><span data-stu-id="97fae-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-findmeetingtimes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="97fae-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="97fae-249">Response</span></span>
<span data-ttu-id="97fae-250">Aqui está uma resposta de exemplo.</span><span class="sxs-lookup"><span data-stu-id="97fae-250">Here is an example response.</span></span> <span data-ttu-id="97fae-251">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="97fae-251">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason": "",
    "meetingTimeSuggestions": [
        {
            "confidence": 100,
            "order": 1,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T17:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 2,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T08:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 3,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T15:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 4,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T10:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 5,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T13:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: user_findmeetingtimes/meetingTimeSuggestions/member/confidence:\r\n    Expected type Double but actual was Int64. Property: confidence, actual value: '100'"
  ]
}
-->


