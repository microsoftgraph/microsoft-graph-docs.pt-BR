---
title: Atualizar outlooktask
description: Alterar as propriedades graváveis de uma tarefa do Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 38d10be1ab316b373b88d0c504998563d67e0792
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053458"
---
# <a name="update-outlooktask-deprecated"></a><span data-ttu-id="19387-103">Atualizar outlooktask (preterido)</span><span class="sxs-lookup"><span data-stu-id="19387-103">Update outlooktask (deprecated)</span></span>

<span data-ttu-id="19387-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19387-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="19387-105">Alterar as propriedades graváveis de uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="19387-105">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="19387-106">A propriedade **completedDateTime** pode ser definida pela ação **Complete** ou explicitamente por uma operação patch.</span><span class="sxs-lookup"><span data-stu-id="19387-106">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="19387-107">Se você usar PATCH para definir **completedDateTime**, certifique-se de definir o **status** `completed` também.</span><span class="sxs-lookup"><span data-stu-id="19387-107">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="19387-108">Por padrão, essa operação (e as operações de tarefa POST, GET e [Complete](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="19387-108">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="19387-109">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="19387-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="19387-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="19387-110">Permissions</span></span>

<span data-ttu-id="19387-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19387-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19387-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19387-113">Permission type</span></span>      | <span data-ttu-id="19387-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19387-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19387-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19387-115">Delegated (work or school account)</span></span> | <span data-ttu-id="19387-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19387-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="19387-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19387-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19387-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19387-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="19387-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19387-119">Application</span></span> | <span data-ttu-id="19387-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19387-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19387-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19387-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="19387-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19387-122">Request headers</span></span>

| <span data-ttu-id="19387-123">Nome</span><span class="sxs-lookup"><span data-stu-id="19387-123">Name</span></span>       | <span data-ttu-id="19387-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="19387-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="19387-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="19387-125">Authorization</span></span>  | <span data-ttu-id="19387-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19387-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19387-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="19387-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="19387-129">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="19387-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="19387-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="19387-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19387-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19387-131">Request body</span></span>

<span data-ttu-id="19387-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="19387-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="19387-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19387-135">Property</span></span> | <span data-ttu-id="19387-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="19387-136">Type</span></span> | <span data-ttu-id="19387-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="19387-137">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="19387-138">body</span><span class="sxs-lookup"><span data-stu-id="19387-138">body</span></span>|[<span data-ttu-id="19387-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="19387-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="19387-140">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-140">The task body that typically contains information about the task.</span></span> <span data-ttu-id="19387-141">Observe para qual tipo de HTML há suporte.</span><span class="sxs-lookup"><span data-stu-id="19387-141">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="19387-142">Categorias</span><span class="sxs-lookup"><span data-stu-id="19387-142">categories</span></span>|<span data-ttu-id="19387-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-143">String collection</span></span>|<span data-ttu-id="19387-144">As categorias associadas à postagem.</span><span class="sxs-lookup"><span data-stu-id="19387-144">The categories associated with the task.</span></span>|
|<span data-ttu-id="19387-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="19387-145">changeKey</span></span>|<span data-ttu-id="19387-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-146">String</span></span>|<span data-ttu-id="19387-147">A versão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-147">The version of the task.</span></span>|
|<span data-ttu-id="19387-148">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="19387-148">completedDateTime</span></span>|[<span data-ttu-id="19387-149">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="19387-149">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="19387-150">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="19387-150">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="19387-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19387-151">createdDateTime</span></span>|<span data-ttu-id="19387-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19387-152">DateTimeOffset</span></span>|<span data-ttu-id="19387-153">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-153">The date and time when the task was created.</span></span> <span data-ttu-id="19387-154">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="19387-154">By default, it is in UTC.</span></span> <span data-ttu-id="19387-155">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19387-155">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="19387-156">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="19387-156">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="19387-157">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="19387-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="19387-158">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="19387-158">dueDateTime</span></span>|[<span data-ttu-id="19387-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="19387-159">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="19387-160">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="19387-160">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="19387-161">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="19387-161">hasAttachments</span></span>|<span data-ttu-id="19387-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="19387-162">Boolean</span></span>|<span data-ttu-id="19387-163">Defina como verdadeiro se a tarefa tiver anexos.</span><span class="sxs-lookup"><span data-stu-id="19387-163">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="19387-164">importance</span><span class="sxs-lookup"><span data-stu-id="19387-164">importance</span></span>|<span data-ttu-id="19387-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-165">string</span></span>|<span data-ttu-id="19387-166">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="19387-166">The importance of the event.</span></span> <span data-ttu-id="19387-167">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="19387-167">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="19387-168">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="19387-168">isReminderOn</span></span>|<span data-ttu-id="19387-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="19387-169">Boolean</span></span>|<span data-ttu-id="19387-170">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-170">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="19387-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19387-171">lastModifiedDateTime</span></span>|<span data-ttu-id="19387-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19387-172">DateTimeOffset</span></span>|<span data-ttu-id="19387-173">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-173">The date and time when the task was last modified.</span></span> <span data-ttu-id="19387-174">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="19387-174">By default, it is in UTC.</span></span> <span data-ttu-id="19387-175">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19387-175">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="19387-176">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="19387-176">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="19387-177">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="19387-177">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="19387-178">proprietário</span><span class="sxs-lookup"><span data-stu-id="19387-178">owner</span></span>|<span data-ttu-id="19387-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-179">String</span></span>|<span data-ttu-id="19387-180">O nome da pessoa que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-180">The name of the person who created the task.</span></span>|
|<span data-ttu-id="19387-181">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="19387-181">parentFolderId</span></span>|<span data-ttu-id="19387-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-182">String</span></span>|<span data-ttu-id="19387-183">O identificador exclusivo para a pasta pai da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-183">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="19387-184">recorrência</span><span class="sxs-lookup"><span data-stu-id="19387-184">recurrence</span></span>|[<span data-ttu-id="19387-185">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="19387-185">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="19387-186">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-186">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="19387-187">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="19387-187">reminderDateTime</span></span>|[<span data-ttu-id="19387-188">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="19387-188">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="19387-189">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-189">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="19387-190">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="19387-190">sensitivity</span></span>|<span data-ttu-id="19387-191">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-191">string</span></span>|<span data-ttu-id="19387-192">Indica o nível de privacidade da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-192">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="19387-193">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="19387-193">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="19387-194">startDateTime</span><span class="sxs-lookup"><span data-stu-id="19387-194">startDateTime</span></span>|[<span data-ttu-id="19387-195">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="19387-195">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="19387-196">A data no fuso horário especificado que a tarefa será iniciada.</span><span class="sxs-lookup"><span data-stu-id="19387-196">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="19387-197">status</span><span class="sxs-lookup"><span data-stu-id="19387-197">status</span></span>|<span data-ttu-id="19387-198">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-198">string</span></span>|<span data-ttu-id="19387-199">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-199">Indicates the state or progress of the task.</span></span> <span data-ttu-id="19387-200">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="19387-200">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="19387-201">assunto</span><span class="sxs-lookup"><span data-stu-id="19387-201">subject</span></span>|<span data-ttu-id="19387-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19387-202">String</span></span>|<span data-ttu-id="19387-203">Uma breve descrição ou o título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="19387-203">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="19387-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="19387-204">Response</span></span>

<span data-ttu-id="19387-205">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTask](../resources/outlooktask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19387-205">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19387-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19387-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="19387-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19387-207">Request</span></span>

<span data-ttu-id="19387-208">O exemplo a seguir modifica a propriedade **dueDateTime** e usa o `Prefer: outlook.timezone` cabeçalho para especificar a expressar as propriedades relacionadas à data na resposta na hora padrão do leste (EST).</span><span class="sxs-lookup"><span data-stu-id="19387-208">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="http"></a>[<span data-ttu-id="19387-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="19387-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19387-210">C#</span><span class="sxs-lookup"><span data-stu-id="19387-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19387-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19387-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19387-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19387-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19387-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="19387-213">Response</span></span>

<span data-ttu-id="19387-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19387-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


