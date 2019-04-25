---
title: Atualizar outlooktask
description: Alterar as propriedades graváveis de uma tarefa do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539786"
---
# <a name="update-outlooktask"></a><span data-ttu-id="a296e-103">Atualizar outlooktask</span><span class="sxs-lookup"><span data-stu-id="a296e-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a296e-104">Alterar as propriedades graváveis de uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a296e-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="a296e-105">A propriedade **completedDateTime** pode ser definida pela ação **Complete** ou explicitamente por uma operação patch.</span><span class="sxs-lookup"><span data-stu-id="a296e-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="a296e-106">Se você usar PATCH para definir **completedDateTime**, certifique-se de \*\*\*\* `completed` definir o status também.</span><span class="sxs-lookup"><span data-stu-id="a296e-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="a296e-107">Por padrão, essa operação (e as operações de tarefa POST, GET e [Complete](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="a296e-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="a296e-108">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="a296e-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="a296e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a296e-109">Permissions</span></span>

<span data-ttu-id="a296e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a296e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a296e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a296e-112">Permission type</span></span>      | <span data-ttu-id="a296e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a296e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a296e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a296e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a296e-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a296e-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a296e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a296e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a296e-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a296e-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a296e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a296e-118">Application</span></span> | <span data-ttu-id="a296e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a296e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a296e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a296e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a296e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a296e-121">Request headers</span></span>

| <span data-ttu-id="a296e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a296e-122">Name</span></span>       | <span data-ttu-id="a296e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a296e-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a296e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a296e-124">Authorization</span></span>  | <span data-ttu-id="a296e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a296e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a296e-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a296e-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a296e-128">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="a296e-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="a296e-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a296e-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a296e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a296e-130">Request body</span></span>

<span data-ttu-id="a296e-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a296e-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a296e-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a296e-134">Property</span></span> | <span data-ttu-id="a296e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="a296e-135">Type</span></span> | <span data-ttu-id="a296e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a296e-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a296e-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a296e-137">assignedTo</span></span>|<span data-ttu-id="a296e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a296e-138">String</span></span>|<span data-ttu-id="a296e-139">O nome da pessoa a qual a tarefa foi atribuída.</span><span class="sxs-lookup"><span data-stu-id="a296e-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="a296e-140">corpo</span><span class="sxs-lookup"><span data-stu-id="a296e-140">body</span></span>|[<span data-ttu-id="a296e-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="a296e-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="a296e-142">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-142">The task body that typically contains information about the task.</span></span> <span data-ttu-id="a296e-143">Observe para qual tipo de HTML há suporte.</span><span class="sxs-lookup"><span data-stu-id="a296e-143">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="a296e-144">categories</span><span class="sxs-lookup"><span data-stu-id="a296e-144">categories</span></span>|<span data-ttu-id="a296e-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a296e-145">String collection</span></span>|<span data-ttu-id="a296e-146">As categorias associadas à postagem.</span><span class="sxs-lookup"><span data-stu-id="a296e-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="a296e-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="a296e-147">changeKey</span></span>|<span data-ttu-id="a296e-148">String</span><span class="sxs-lookup"><span data-stu-id="a296e-148">String</span></span>|<span data-ttu-id="a296e-149">A versão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-149">The version of the task.</span></span>|
|<span data-ttu-id="a296e-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="a296e-150">completedDateTime</span></span>|[<span data-ttu-id="a296e-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a296e-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a296e-152">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="a296e-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="a296e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a296e-153">createdDateTime</span></span>|<span data-ttu-id="a296e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a296e-154">DateTimeOffset</span></span>|<span data-ttu-id="a296e-155">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-155">The date and time when the task was created.</span></span> <span data-ttu-id="a296e-156">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="a296e-156">By default, it is in UTC.</span></span> <span data-ttu-id="a296e-157">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a296e-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="a296e-158">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="a296e-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="a296e-159">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a296e-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a296e-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a296e-160">dueDateTime</span></span>|[<span data-ttu-id="a296e-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a296e-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a296e-162">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="a296e-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="a296e-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="a296e-163">hasAttachments</span></span>|<span data-ttu-id="a296e-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="a296e-164">Boolean</span></span>|<span data-ttu-id="a296e-165">Defina como verdadeiro se a tarefa tiver anexos.</span><span class="sxs-lookup"><span data-stu-id="a296e-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="a296e-166">importance</span><span class="sxs-lookup"><span data-stu-id="a296e-166">importance</span></span>|<span data-ttu-id="a296e-167">string</span><span class="sxs-lookup"><span data-stu-id="a296e-167">string</span></span>|<span data-ttu-id="a296e-168">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="a296e-168">The importance of the event.</span></span> <span data-ttu-id="a296e-169">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a296e-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="a296e-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="a296e-170">isReminderOn</span></span>|<span data-ttu-id="a296e-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="a296e-171">Boolean</span></span>|<span data-ttu-id="a296e-172">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="a296e-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a296e-173">lastModifiedDateTime</span></span>|<span data-ttu-id="a296e-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a296e-174">DateTimeOffset</span></span>|<span data-ttu-id="a296e-175">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="a296e-176">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="a296e-176">By default, it is in UTC.</span></span> <span data-ttu-id="a296e-177">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a296e-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="a296e-178">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a296e-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a296e-179">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a296e-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a296e-180">proprietário</span><span class="sxs-lookup"><span data-stu-id="a296e-180">owner</span></span>|<span data-ttu-id="a296e-181">String</span><span class="sxs-lookup"><span data-stu-id="a296e-181">String</span></span>|<span data-ttu-id="a296e-182">O nome da pessoa que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="a296e-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="a296e-183">parentFolderId</span></span>|<span data-ttu-id="a296e-184">String</span><span class="sxs-lookup"><span data-stu-id="a296e-184">String</span></span>|<span data-ttu-id="a296e-185">O identificador exclusivo para a pasta pai da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="a296e-186">recorrência</span><span class="sxs-lookup"><span data-stu-id="a296e-186">recurrence</span></span>|[<span data-ttu-id="a296e-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a296e-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="a296e-188">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="a296e-189">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="a296e-189">reminderDateTime</span></span>|[<span data-ttu-id="a296e-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a296e-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a296e-191">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="a296e-192">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="a296e-192">sensitivity</span></span>|<span data-ttu-id="a296e-193">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a296e-193">string</span></span>|<span data-ttu-id="a296e-194">Indica o nível de privacidade da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="a296e-195">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="a296e-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="a296e-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a296e-196">startDateTime</span></span>|[<span data-ttu-id="a296e-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a296e-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a296e-198">A data no fuso horário especificado que a tarefa será iniciada.</span><span class="sxs-lookup"><span data-stu-id="a296e-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="a296e-199">status</span><span class="sxs-lookup"><span data-stu-id="a296e-199">status</span></span>|<span data-ttu-id="a296e-200">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a296e-200">string</span></span>|<span data-ttu-id="a296e-201">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="a296e-202">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="a296e-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="a296e-203">subject</span><span class="sxs-lookup"><span data-stu-id="a296e-203">subject</span></span>|<span data-ttu-id="a296e-204">String</span><span class="sxs-lookup"><span data-stu-id="a296e-204">String</span></span>|<span data-ttu-id="a296e-205">Uma breve descrição ou o título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="a296e-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="a296e-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="a296e-206">Response</span></span>

<span data-ttu-id="a296e-207">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTask](../resources/outlooktask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a296e-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a296e-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a296e-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="a296e-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a296e-209">Request</span></span>

<span data-ttu-id="a296e-210">O exemplo a seguir modifica a propriedade **dueDateTime** e usa o `Prefer: outlook.timezone` cabeçalho para especificar a expressar as propriedades relacionadas à data na resposta na hora padrão do leste (EST).</span><span class="sxs-lookup"><span data-stu-id="a296e-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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

### <a name="response"></a><span data-ttu-id="a296e-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="a296e-211">Response</span></span>

<span data-ttu-id="a296e-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a296e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
