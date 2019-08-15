---
title: Atualizar outlooktask
description: Alterar as propriedades graváveis de uma tarefa do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e2f3d77ef33e900b506547792f4cfe7061f78404
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414102"
---
# <a name="update-outlooktask"></a><span data-ttu-id="02070-103">Atualizar outlooktask</span><span class="sxs-lookup"><span data-stu-id="02070-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02070-104">Alterar as propriedades graváveis de uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="02070-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="02070-105">A propriedade **completedDateTime** pode ser definida pela ação **Complete** ou explicitamente por uma operação patch.</span><span class="sxs-lookup"><span data-stu-id="02070-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="02070-106">Se você usar PATCH para definir **completedDateTime**, certifique-se de \*\*\*\* `completed` definir o status também.</span><span class="sxs-lookup"><span data-stu-id="02070-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="02070-107">Por padrão, essa operação (e as operações de tarefa POST, GET e [Complete](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="02070-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="02070-108">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="02070-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="02070-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="02070-109">Permissions</span></span>

<span data-ttu-id="02070-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02070-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02070-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02070-112">Permission type</span></span>      | <span data-ttu-id="02070-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02070-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02070-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02070-114">Delegated (work or school account)</span></span> | <span data-ttu-id="02070-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02070-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="02070-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02070-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02070-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02070-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="02070-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02070-118">Application</span></span> | <span data-ttu-id="02070-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02070-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02070-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02070-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="02070-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02070-121">Request headers</span></span>

| <span data-ttu-id="02070-122">Nome</span><span class="sxs-lookup"><span data-stu-id="02070-122">Name</span></span>       | <span data-ttu-id="02070-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="02070-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02070-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="02070-124">Authorization</span></span>  | <span data-ttu-id="02070-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02070-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02070-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="02070-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="02070-128">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="02070-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="02070-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02070-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02070-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02070-130">Request body</span></span>

<span data-ttu-id="02070-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="02070-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="02070-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02070-134">Property</span></span> | <span data-ttu-id="02070-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="02070-135">Type</span></span> | <span data-ttu-id="02070-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="02070-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="02070-137">corpo</span><span class="sxs-lookup"><span data-stu-id="02070-137">body</span></span>|[<span data-ttu-id="02070-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="02070-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="02070-139">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="02070-140">Observe para qual tipo de HTML há suporte.</span><span class="sxs-lookup"><span data-stu-id="02070-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="02070-141">Categorias</span><span class="sxs-lookup"><span data-stu-id="02070-141">categories</span></span>|<span data-ttu-id="02070-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02070-142">String collection</span></span>|<span data-ttu-id="02070-143">As categorias associadas à postagem.</span><span class="sxs-lookup"><span data-stu-id="02070-143">The categories associated with the task.</span></span>|
|<span data-ttu-id="02070-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="02070-144">changeKey</span></span>|<span data-ttu-id="02070-145">String</span><span class="sxs-lookup"><span data-stu-id="02070-145">String</span></span>|<span data-ttu-id="02070-146">A versão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-146">The version of the task.</span></span>|
|<span data-ttu-id="02070-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="02070-147">completedDateTime</span></span>|[<span data-ttu-id="02070-148">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02070-148">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02070-149">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="02070-149">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="02070-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02070-150">createdDateTime</span></span>|<span data-ttu-id="02070-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02070-151">DateTimeOffset</span></span>|<span data-ttu-id="02070-152">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-152">The date and time when the task was created.</span></span> <span data-ttu-id="02070-153">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="02070-153">By default, it is in UTC.</span></span> <span data-ttu-id="02070-154">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02070-154">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="02070-155">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="02070-155">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="02070-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="02070-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="02070-157">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="02070-157">dueDateTime</span></span>|[<span data-ttu-id="02070-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02070-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02070-159">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="02070-159">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="02070-160">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="02070-160">hasAttachments</span></span>|<span data-ttu-id="02070-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="02070-161">Boolean</span></span>|<span data-ttu-id="02070-162">Defina como verdadeiro se a tarefa tiver anexos.</span><span class="sxs-lookup"><span data-stu-id="02070-162">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="02070-163">importance</span><span class="sxs-lookup"><span data-stu-id="02070-163">importance</span></span>|<span data-ttu-id="02070-164">string</span><span class="sxs-lookup"><span data-stu-id="02070-164">string</span></span>|<span data-ttu-id="02070-165">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="02070-165">The importance of the event.</span></span> <span data-ttu-id="02070-166">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="02070-166">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="02070-167">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="02070-167">isReminderOn</span></span>|<span data-ttu-id="02070-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="02070-168">Boolean</span></span>|<span data-ttu-id="02070-169">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-169">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="02070-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02070-170">lastModifiedDateTime</span></span>|<span data-ttu-id="02070-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02070-171">DateTimeOffset</span></span>|<span data-ttu-id="02070-172">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-172">The date and time when the task was last modified.</span></span> <span data-ttu-id="02070-173">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="02070-173">By default, it is in UTC.</span></span> <span data-ttu-id="02070-174">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02070-174">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="02070-175">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="02070-175">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="02070-176">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="02070-176">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="02070-177">proprietário</span><span class="sxs-lookup"><span data-stu-id="02070-177">owner</span></span>|<span data-ttu-id="02070-178">String</span><span class="sxs-lookup"><span data-stu-id="02070-178">String</span></span>|<span data-ttu-id="02070-179">O nome da pessoa que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-179">The name of the person who created the task.</span></span>|
|<span data-ttu-id="02070-180">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="02070-180">parentFolderId</span></span>|<span data-ttu-id="02070-181">String</span><span class="sxs-lookup"><span data-stu-id="02070-181">String</span></span>|<span data-ttu-id="02070-182">O identificador exclusivo para a pasta pai da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-182">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="02070-183">recorrência</span><span class="sxs-lookup"><span data-stu-id="02070-183">recurrence</span></span>|[<span data-ttu-id="02070-184">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="02070-184">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="02070-185">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-185">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="02070-186">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="02070-186">reminderDateTime</span></span>|[<span data-ttu-id="02070-187">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02070-187">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02070-188">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-188">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="02070-189">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="02070-189">sensitivity</span></span>|<span data-ttu-id="02070-190">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02070-190">string</span></span>|<span data-ttu-id="02070-191">Indica o nível de privacidade da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-191">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="02070-192">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="02070-192">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="02070-193">startDateTime</span><span class="sxs-lookup"><span data-stu-id="02070-193">startDateTime</span></span>|[<span data-ttu-id="02070-194">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02070-194">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02070-195">A data no fuso horário especificado que a tarefa será iniciada.</span><span class="sxs-lookup"><span data-stu-id="02070-195">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="02070-196">status</span><span class="sxs-lookup"><span data-stu-id="02070-196">status</span></span>|<span data-ttu-id="02070-197">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02070-197">string</span></span>|<span data-ttu-id="02070-198">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-198">Indicates the state or progress of the task.</span></span> <span data-ttu-id="02070-199">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="02070-199">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="02070-200">assunto</span><span class="sxs-lookup"><span data-stu-id="02070-200">subject</span></span>|<span data-ttu-id="02070-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02070-201">String</span></span>|<span data-ttu-id="02070-202">Uma breve descrição ou o título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="02070-202">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="02070-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="02070-203">Response</span></span>

<span data-ttu-id="02070-204">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTask](../resources/outlooktask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02070-204">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02070-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02070-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="02070-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02070-206">Request</span></span>

<span data-ttu-id="02070-207">O exemplo a seguir modifica a propriedade **dueDateTime** e usa o `Prefer: outlook.timezone` cabeçalho para especificar a expressar as propriedades relacionadas à data na resposta na hora padrão do leste (EST).</span><span class="sxs-lookup"><span data-stu-id="02070-207">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02070-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="02070-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTHgwAAA=
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="02070-209">C#</span><span class="sxs-lookup"><span data-stu-id="02070-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02070-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02070-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02070-211">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="02070-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02070-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="02070-212">Response</span></span>

<span data-ttu-id="02070-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02070-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
