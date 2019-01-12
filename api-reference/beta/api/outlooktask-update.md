---
title: Atualizar outlooktask
description: Alterar propriedades graváveis de uma tarefa do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c0d2ff13f3e7971e686389709fbdde027458ef67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964932"
---
# <a name="update-outlooktask"></a><span data-ttu-id="e07a3-103">Atualizar outlooktask</span><span class="sxs-lookup"><span data-stu-id="e07a3-103">Update outlooktask</span></span>

> <span data-ttu-id="e07a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e07a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e07a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e07a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e07a3-106">Alterar propriedades graváveis de uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e07a3-106">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="e07a3-107">A propriedade **completedDateTime** pode ser definida pela ação **completa** ou explicitamente por uma operação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="e07a3-107">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="e07a3-108">Se você usar o PATCH para definir **completedDateTime**, verifique se você definir **status** como `completed` também.</span><span class="sxs-lookup"><span data-stu-id="e07a3-108">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="e07a3-109">Por padrão, esta operação (e as operações de tarefa POST, GET e [Concluir](../api/outlooktask-complete.md) ) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="e07a3-109">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="e07a3-110">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="e07a3-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="e07a3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e07a3-111">Permissions</span></span>

<span data-ttu-id="e07a3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e07a3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e07a3-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e07a3-114">Permission type</span></span>      | <span data-ttu-id="e07a3-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e07a3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e07a3-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e07a3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e07a3-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e07a3-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e07a3-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e07a3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e07a3-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e07a3-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e07a3-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e07a3-120">Application</span></span> | <span data-ttu-id="e07a3-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e07a3-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e07a3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e07a3-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e07a3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e07a3-123">Request headers</span></span>

| <span data-ttu-id="e07a3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e07a3-124">Name</span></span>       | <span data-ttu-id="e07a3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e07a3-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e07a3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e07a3-126">Authorization</span></span>  | <span data-ttu-id="e07a3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e07a3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e07a3-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e07a3-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e07a3-130">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="e07a3-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="e07a3-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e07a3-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e07a3-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e07a3-132">Request body</span></span>

<span data-ttu-id="e07a3-p107">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e07a3-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e07a3-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e07a3-136">Property</span></span> | <span data-ttu-id="e07a3-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="e07a3-137">Type</span></span> | <span data-ttu-id="e07a3-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e07a3-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e07a3-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="e07a3-139">assignedTo</span></span>|<span data-ttu-id="e07a3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07a3-140">String</span></span>|<span data-ttu-id="e07a3-141">O nome da pessoa que tenha sido atribuído a tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-141">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="e07a3-142">body</span><span class="sxs-lookup"><span data-stu-id="e07a3-142">body</span></span>|[<span data-ttu-id="e07a3-143">itemBody</span><span class="sxs-lookup"><span data-stu-id="e07a3-143">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="e07a3-144">O corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-144">The task body that typically contains information about the task.</span></span> <span data-ttu-id="e07a3-145">Observe que apenas o tipo de HTML é suportado.</span><span class="sxs-lookup"><span data-stu-id="e07a3-145">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="e07a3-146">categories</span><span class="sxs-lookup"><span data-stu-id="e07a3-146">categories</span></span>|<span data-ttu-id="e07a3-147">String collection</span><span class="sxs-lookup"><span data-stu-id="e07a3-147">String collection</span></span>|<span data-ttu-id="e07a3-148">As categorias associadas à tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-148">The categories associated with the task.</span></span>|
|<span data-ttu-id="e07a3-149">changeKey</span><span class="sxs-lookup"><span data-stu-id="e07a3-149">changeKey</span></span>|<span data-ttu-id="e07a3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07a3-150">String</span></span>|<span data-ttu-id="e07a3-151">A versão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-151">The version of the task.</span></span>|
|<span data-ttu-id="e07a3-152">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e07a3-152">completedDateTime</span></span>|[<span data-ttu-id="e07a3-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e07a3-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e07a3-154">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="e07a3-154">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="e07a3-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e07a3-155">createdDateTime</span></span>|<span data-ttu-id="e07a3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07a3-156">DateTimeOffset</span></span>|<span data-ttu-id="e07a3-157">A data e hora em que a tarefa foi criada.</span><span class="sxs-lookup"><span data-stu-id="e07a3-157">The date and time when the task was created.</span></span> <span data-ttu-id="e07a3-158">Por padrão, ela é em UTC.</span><span class="sxs-lookup"><span data-stu-id="e07a3-158">By default, it is in UTC.</span></span> <span data-ttu-id="e07a3-159">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e07a3-159">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e07a3-160">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e07a3-160">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="e07a3-161">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e07a3-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e07a3-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e07a3-162">dueDateTime</span></span>|[<span data-ttu-id="e07a3-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e07a3-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e07a3-164">A data em que o fuso horário especificado que a tarefa deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="e07a3-164">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="e07a3-165">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e07a3-165">hasAttachments</span></span>|<span data-ttu-id="e07a3-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="e07a3-166">Boolean</span></span>|<span data-ttu-id="e07a3-167">Defina como true se a tarefa tiver anexos.</span><span class="sxs-lookup"><span data-stu-id="e07a3-167">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="e07a3-168">importance</span><span class="sxs-lookup"><span data-stu-id="e07a3-168">importance</span></span>|<span data-ttu-id="e07a3-169">string</span><span class="sxs-lookup"><span data-stu-id="e07a3-169">string</span></span>|<span data-ttu-id="e07a3-170">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="e07a3-170">The importance of the event.</span></span> <span data-ttu-id="e07a3-171">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e07a3-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="e07a3-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="e07a3-172">isReminderOn</span></span>|<span data-ttu-id="e07a3-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="e07a3-173">Boolean</span></span>|<span data-ttu-id="e07a3-174">Defina como true se um alerta for definido como lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="e07a3-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e07a3-175">lastModifiedDateTime</span></span>|<span data-ttu-id="e07a3-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07a3-176">DateTimeOffset</span></span>|<span data-ttu-id="e07a3-177">A data e a hora da última modificação a tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="e07a3-178">Por padrão, ela é em UTC.</span><span class="sxs-lookup"><span data-stu-id="e07a3-178">By default, it is in UTC.</span></span> <span data-ttu-id="e07a3-179">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e07a3-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e07a3-180">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e07a3-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e07a3-181">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e07a3-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e07a3-182">owner</span><span class="sxs-lookup"><span data-stu-id="e07a3-182">owner</span></span>|<span data-ttu-id="e07a3-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07a3-183">String</span></span>|<span data-ttu-id="e07a3-184">O nome da pessoa que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-184">The name of the person who created the task.</span></span>|
|<span data-ttu-id="e07a3-185">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e07a3-185">parentFolderId</span></span>|<span data-ttu-id="e07a3-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07a3-186">String</span></span>|<span data-ttu-id="e07a3-187">O identificador exclusivo para a pasta do pai da tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-187">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="e07a3-188">recurrence</span><span class="sxs-lookup"><span data-stu-id="e07a3-188">recurrence</span></span>|[<span data-ttu-id="e07a3-189">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e07a3-189">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="e07a3-190">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-190">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="e07a3-191">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="e07a3-191">reminderDateTime</span></span>|[<span data-ttu-id="e07a3-192">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e07a3-192">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e07a3-193">A data e hora para um alerta de lembrete da tarefa ocorra.</span><span class="sxs-lookup"><span data-stu-id="e07a3-193">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="e07a3-194">sensitivity</span><span class="sxs-lookup"><span data-stu-id="e07a3-194">sensitivity</span></span>|<span data-ttu-id="e07a3-195">string</span><span class="sxs-lookup"><span data-stu-id="e07a3-195">string</span></span>|<span data-ttu-id="e07a3-196">Indica o nível de privacidade para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-196">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="e07a3-197">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="e07a3-197">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="e07a3-198">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e07a3-198">startDateTime</span></span>|[<span data-ttu-id="e07a3-199">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e07a3-199">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e07a3-200">A data no fuso horário especificado quando a tarefa for começar.</span><span class="sxs-lookup"><span data-stu-id="e07a3-200">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="e07a3-201">status</span><span class="sxs-lookup"><span data-stu-id="e07a3-201">status</span></span>|<span data-ttu-id="e07a3-202">string</span><span class="sxs-lookup"><span data-stu-id="e07a3-202">string</span></span>|<span data-ttu-id="e07a3-203">Indica o estado ou o progresso da tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-203">Indicates the state or progress of the task.</span></span> <span data-ttu-id="e07a3-204">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="e07a3-204">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="e07a3-205">subject</span><span class="sxs-lookup"><span data-stu-id="e07a3-205">subject</span></span>|<span data-ttu-id="e07a3-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07a3-206">String</span></span>|<span data-ttu-id="e07a3-207">Uma breve descrição ou o título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="e07a3-207">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="e07a3-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="e07a3-208">Response</span></span>

<span data-ttu-id="e07a3-209">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e07a3-209">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e07a3-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e07a3-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="e07a3-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e07a3-211">Request</span></span>

<span data-ttu-id="e07a3-212">O exemplo a seguir modifica a propriedade **dueDateTime** e usa o `Prefer: outlook.timezone` cabeçalho para especificar expressar as propriedades relacionadas a data em que a resposta na hora padrão do Leste (EST).</span><span class="sxs-lookup"><span data-stu-id="e07a3-212">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a><span data-ttu-id="e07a3-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="e07a3-213">Response</span></span>

<span data-ttu-id="e07a3-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e07a3-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
