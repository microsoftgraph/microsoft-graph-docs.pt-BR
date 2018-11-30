---
title: 'user: findMeetingTimes'
description: Sugerir horários de reunião e com base na disponibilidade do organizador e participante e restrições de tempo ou o local especificadas como parâmetros de locais.
ms.openlocfilehash: 7ee6794041310d031f257bb83714de57f4af0cee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003628"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="1ecf9-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="1ecf9-103">user: findMeetingTimes</span></span>
<span data-ttu-id="1ecf9-104">Sugerir horários de reunião e com base na disponibilidade do organizador e participante e restrições de tempo ou o local especificadas como parâmetros de locais.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-104">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="1ecf9-p101">Se **findMeetingTimes** não retorna nenhuma sugestão de reunião, a resposta seria indicar um motivo na propriedade **emptySuggestionsReason**. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>


## <a name="permissions"></a><span data-ttu-id="1ecf9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ecf9-107">Permissions</span></span>
<span data-ttu-id="1ecf9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ecf9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ecf9-110">Permission type</span></span>      | <span data-ttu-id="1ecf9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ecf9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ecf9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ecf9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ecf9-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="1ecf9-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="1ecf9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ecf9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ecf9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-115">Not supported.</span></span>    |
|<span data-ttu-id="1ecf9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ecf9-116">Application</span></span> | <span data-ttu-id="1ecf9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ecf9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ecf9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="1ecf9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecf9-119">Request headers</span></span>
| <span data-ttu-id="1ecf9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1ecf9-120">Name</span></span>       | <span data-ttu-id="1ecf9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ecf9-121">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ecf9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ecf9-122">Authorization</span></span>  | <span data-ttu-id="1ecf9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ecf9-125">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1ecf9-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="1ecf9-p104">Uma cadeia de caracteres que representa um fuso horário específico para a resposta; por exemplo, "Hora Oficial do Pacífico". Opcional. UTC será usado se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p104">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ecf9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecf9-129">Request body</span></span>
<span data-ttu-id="1ecf9-p105">Todos os parâmetros suportados estão listados abaixo. Dependendo do cenário, especifique um objeto JSON para cada um dos parâmetros necessários no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p105">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="1ecf9-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1ecf9-132">Parameter</span></span>    | <span data-ttu-id="1ecf9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ecf9-133">Type</span></span>   |<span data-ttu-id="1ecf9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ecf9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ecf9-135">attendees</span><span class="sxs-lookup"><span data-stu-id="1ecf9-135">attendees</span></span>|<span data-ttu-id="1ecf9-136">Coleção [attendeeBase](../resources/attendeebase.md)</span><span class="sxs-lookup"><span data-stu-id="1ecf9-136">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="1ecf9-p106">Uma coleção de participantes ou recursos da reunião. Como findMeetingTimes pressupõe que qualquer participante que seja uma pessoa será sempre obrigatório, especifique `required` para uma pessoa e `resource` para um recurso na propriedade **type** correspondente. Uma coleção vazia faz com que **findMeetingTimes** procure gratuitamente alocações de tempo somente para o organizador. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p106">A collection of attendees or resources for the meeting. Since findMeetingTimes assumes that any attendee who is a person is always required, specify `required` for a person and `resource` for a resource in the corresponding **type** property. An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer. Optional.</span></span>|
|<span data-ttu-id="1ecf9-141">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="1ecf9-141">isOrganizerOptional</span></span>|<span data-ttu-id="1ecf9-142">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecf9-142">Edm.Boolean</span></span>|<span data-ttu-id="1ecf9-p107">Especifique `True` se o organizador não tiver necessariamente que participar. O padrão é `false`. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p107">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="1ecf9-146">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="1ecf9-146">locationConstraint</span></span>|[<span data-ttu-id="1ecf9-147">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="1ecf9-147">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="1ecf9-p108">Os requisitos do organizador sobre o local da reunião, tal como se é necessário sugerir de um local de encontro, ou há locais específicos apenas onde a reunião pode ocorrer. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p108">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="1ecf9-150">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="1ecf9-150">maxCandidates</span></span>|<span data-ttu-id="1ecf9-151">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1ecf9-151">Edm.Int32</span></span>|<span data-ttu-id="1ecf9-p109">O número máximo de sugestões de horários de reunião a ser retornados. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p109">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="1ecf9-154">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="1ecf9-154">meetingDuration</span></span>|<span data-ttu-id="1ecf9-155">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="1ecf9-155">Edm.Duration</span></span>|<span data-ttu-id="1ecf9-p110">A duração da reunião, indicada no formato [ISO8601](https://www.iso.org/iso/iso8601). Por exemplo, 1 hora é indicada como "PT1H", onde "P" é o designador de duração, "T" é o designador de horário e "H" é o designador de hora. Use M para indicar os minutos da duração; por exemplo, 2 horas e 30 minutos seria “PT2H30M”. Se a duração da reunião não for especificada, **findMeetingTimes** usará o padrão de 30 minutos. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p110">The length of the meeting, denoted in [ISO8601](https://www.iso.org/iso/iso8601) format. For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator. Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'. If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes. Optional.</span></span>|
|<span data-ttu-id="1ecf9-161">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="1ecf9-161">minimumAttendeePercentage</span></span>|<span data-ttu-id="1ecf9-162">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="1ecf9-162">Edm.Double</span></span>| <span data-ttu-id="1ecf9-p111">O mínimo necessário de [confiança](#the-confidence-of-a-meeting-suggestion) para um intervalo de tempo a ser retornado na resposta. É um valor de % variando de 0 a 100. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p111">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="1ecf9-166">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="1ecf9-166">returnSuggestionReasons</span></span>|<span data-ttu-id="1ecf9-167">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecf9-167">Edm.Boolean</span></span>|<span data-ttu-id="1ecf9-p112">Especifique `True` para retornar um motivo para cada sugestão de reunião na propriedade **suggestionReason**. O padrão é `false` para não retornar essa propriedade. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p112">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="1ecf9-171">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="1ecf9-171">timeConstraint</span></span>|[<span data-ttu-id="1ecf9-172">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="1ecf9-172">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="1ecf9-p113">Qualquer restrição de tempo para uma reunião, o que pode incluir a natureza da reunião (propriedade **activityDomain**) e possíveis intervalos de tempo da reunião (propriedade **timeSlots**). **findMeetingTimes** pressupõe **activityDomain** como `work` se você não especificar este parâmetro. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p113">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="1ecf9-176">A tabela a seguir descreve as restrições de **activityDomain** , que você poderá ampliar a especificação no parâmetro **timeConstraint** .</span><span class="sxs-lookup"><span data-stu-id="1ecf9-176">The following table describes the **activityDomain** restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="1ecf9-177">valor de activityDomain</span><span class="sxs-lookup"><span data-stu-id="1ecf9-177">activityDomain value</span></span>|<span data-ttu-id="1ecf9-178">Sugestões de horário para reuniões</span><span class="sxs-lookup"><span data-stu-id="1ecf9-178">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ecf9-179">trabalho</span><span class="sxs-lookup"><span data-stu-id="1ecf9-179">work</span></span>| <span data-ttu-id="1ecf9-p114">As sugestões são nas horas de trabalho do usuário que são definidas na configuração do calendário do usuário e podem ser personalizadas pelo usuário ou administrador. As horas de trabalho padrão são de segunda a sexta, das 8h às 17h, no fuso horário definido para a caixa de correio. Este é o valor padrão se nenhum **activityDomain** for especificado.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p114">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="1ecf9-183">pessoal</span><span class="sxs-lookup"><span data-stu-id="1ecf9-183">personal</span></span>| <span data-ttu-id="1ecf9-p115">As sugestões são dentro das horas de trabalho do usuário, e sábado e domingo. O padrão é de segunda a sexta, das 8h às 17h, na configuração de fuso horário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p115">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="1ecf9-186">irrestrito</span><span class="sxs-lookup"><span data-stu-id="1ecf9-186">unrestricted</span></span> | <span data-ttu-id="1ecf9-187">As sugestões podem ser todas as horas do dia, todos os dias da semana.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-187">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="1ecf9-188">desconhecido</span><span class="sxs-lookup"><span data-stu-id="1ecf9-188">unknown</span></span> | <span data-ttu-id="1ecf9-p116">Não use esse valor, uma vez que ele será substituído no futuro. Atualmente, se comporta da mesma forma que o `work`. Altere qualquer código existente para usar o `work`, `personal` ou `unrestricted` conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p116">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>


<span data-ttu-id="1ecf9-p117">Com base nos parâmetros especificados,**findMeetingTimes** verifica o status disponível/ocupado nos calendários principais do organizador e dos participantes. A ação calcula os melhores possíveis horários de reuniões e retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p117">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="1ecf9-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ecf9-194">Response</span></span>

<span data-ttu-id="1ecf9-195">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-195">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="1ecf9-p118">Um **meetingTimeSuggestionsResult** inclui uma coleção de sugestões de reunião e uma propriedade **emptySuggestionsReason**. Cada sugestão é definida como uma [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), e participantes com um nível de confiança de 50% na média para participar ou uma % específica que definida no parâmetro **minimumAttendeePercentage**.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p118">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="1ecf9-198">Por padrão, cada sugestão de horário de reunião é retornado em UTC.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-198">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="1ecf9-p119">Se **findMeetingTimes** não retorna nenhuma sugestão de reunião, a resposta seria indicar um motivo na propriedade **emptySuggestionsReason**. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p119">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="1ecf9-201">A confiança de uma sugestão de reunião</span><span class="sxs-lookup"><span data-stu-id="1ecf9-201">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="1ecf9-202">A propriedade **confidence** de uma **meetingTimeSuggestion** varia de 0% a 100% e representa a chance de que todos os participantes compareçam à reunião, com base em seu status disponível/ocupado:</span><span class="sxs-lookup"><span data-stu-id="1ecf9-202">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="1ecf9-203">Para cada participante, um status livre para um período de tempo de reunião especificado corresponde à chance de 100% de presença, status desconhecido 49% e status ocupado 0%.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-203">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="1ecf9-204">A confiança na sugestão de um horário de reunião é calculada pela média da chance de presença de todos os participantes especificados para essa reunião.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-204">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="1ecf9-p120">Você pode usar o parâmetro opcional **minimumAttendeePercentage** **findMeetingTimes** para especificar que apenas as sugestões de horário da reunião com pelo menos determinado nível de confiança retornem. Por exemplo, você pode especificar uma **minimumAttendeePercentage** de 80% se você quiser apenas sugestões que tenham uma chance de 80% ou mais de que todos os participantes comparecerão. Se você não especificar **minimumAttendeePercentage**, **findMeetingTimes** pressupõe um valor de 50%.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p120">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>
- <span data-ttu-id="1ecf9-p121">Se houver diversas sugestões de horário de reunião, a ação **findMeetingTimes** primeiramente classifica as sugestões por seu valor de confiança computado que vai de alto para baixo. Se houver sugestões com a mesma confiança, a ação ordena essas sugestões em ordem cronológica.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>

<span data-ttu-id="1ecf9-210">Por exemplo, se uma sugestão de horário de reunião envolve três participantes com o seguinte status livre/ocupado:</span><span class="sxs-lookup"><span data-stu-id="1ecf9-210">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="1ecf9-211">**Participante**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-211">**Attendee**</span></span>|<span data-ttu-id="1ecf9-212">**Status disponível/ocupado**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-212">**Free/busy status**</span></span>|<span data-ttu-id="1ecf9-213">**% de chance de comparecer**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-213">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ecf9-214">Sara</span><span class="sxs-lookup"><span data-stu-id="1ecf9-214">Dana</span></span> | <span data-ttu-id="1ecf9-215">Disponível</span><span class="sxs-lookup"><span data-stu-id="1ecf9-215">Free</span></span> | <span data-ttu-id="1ecf9-216">100%</span><span class="sxs-lookup"><span data-stu-id="1ecf9-216">100%</span></span> |
|<span data-ttu-id="1ecf9-217">Davi</span><span class="sxs-lookup"><span data-stu-id="1ecf9-217">John</span></span> | <span data-ttu-id="1ecf9-218">Desconhecido</span><span class="sxs-lookup"><span data-stu-id="1ecf9-218">Unknown</span></span> | <span data-ttu-id="1ecf9-219">49%</span><span class="sxs-lookup"><span data-stu-id="1ecf9-219">49%</span></span> |
|<span data-ttu-id="1ecf9-220">Sara</span><span class="sxs-lookup"><span data-stu-id="1ecf9-220">Samantha</span></span> | <span data-ttu-id="1ecf9-221">Ocupado</span><span class="sxs-lookup"><span data-stu-id="1ecf9-221">Busy</span></span> | <span data-ttu-id="1ecf9-222">0%</span><span class="sxs-lookup"><span data-stu-id="1ecf9-222">0%</span></span> |

<span data-ttu-id="1ecf9-223">Então a confiança na sugestão do horário da reunião, que corresponde à chance média de presença, é (100% + 49% + 0%) /3 = 49.66%.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-223">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="1ecf9-224">Se você especificar um **minimumAttendeePercentage** de 80% em uma operação **findMeetingTimes**, pois 49,66%< 80%, a operação não sugerirá esse horário na resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-224">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="1ecf9-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ecf9-225">Example</span></span>

<span data-ttu-id="1ecf9-226">O exemplo a seguir mostra como encontrar um horário para reunir-se em um local predeterminado e solicitar um motivo para cada sugestão, especificando os seguintes parâmetros no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="1ecf9-226">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="1ecf9-227">**attendees**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-227">**attendees**</span></span>
- <span data-ttu-id="1ecf9-228">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-228">**locationConstraint**</span></span>
- <span data-ttu-id="1ecf9-229">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-229">**timeConstraint**</span></span>
- <span data-ttu-id="1ecf9-230">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-230">**meetingDuration**</span></span>
- <span data-ttu-id="1ecf9-231">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-231">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="1ecf9-232">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="1ecf9-232">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="1ecf9-233">Definindo o parâmetro **returnSuggestionReasons**, você também obtém uma explicação na propriedade **suggestionReason** para cada sugestão, se **findMeetingTimes** retornar qualquer sugestão.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-233">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="1ecf9-p122">Observe que a solicitação especifica o horário no fuso Horário Padrão do Pacífico e a resposta retorna as sugestões de horário da reunião em UTC, por padrão. Você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar os valores de horário para o Horário Padrão do Pacífico na resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p122">Notice that the request specifies time in the PST time zone, and the response returns meeting time suggestions in UTC, by default. You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="1ecf9-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecf9-236">Request</span></span>
<span data-ttu-id="1ecf9-237">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-237">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
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
    "activityDomain":"unrestricted", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-17T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-19T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100.0
}
```

##### <a name="response"></a><span data-ttu-id="1ecf9-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ecf9-238">Response</span></span>
<span data-ttu-id="1ecf9-p123">Aqui está uma resposta de exemplo. Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ecf9-p123">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
Content-Length: 976

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T18:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        },
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T22:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/user-findmeetingtimes.md:
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|"
  ],
  "tocPath": ""
}-->
