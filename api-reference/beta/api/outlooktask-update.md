---
title: Atualizar outlooktask
description: Alterar as propriedades graváveis de uma tarefa do Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3225fd6249cad572d29f3f11175369d183b40dd0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978785"
---
# <a name="update-outlooktask-deprecated"></a><span data-ttu-id="53026-103">Atualizar outlooktask (preterido)</span><span class="sxs-lookup"><span data-stu-id="53026-103">Update outlooktask (deprecated)</span></span>

<span data-ttu-id="53026-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53026-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="53026-105">Alterar as propriedades graváveis de uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="53026-105">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="53026-106">A propriedade **completedDateTime** pode ser definida pela ação **Complete** ou explicitamente por uma operação patch.</span><span class="sxs-lookup"><span data-stu-id="53026-106">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="53026-107">Se você usar PATCH para definir **completedDateTime** , certifique-se de definir o **status** `completed` também.</span><span class="sxs-lookup"><span data-stu-id="53026-107">If you use PATCH to set **completedDateTime** , make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="53026-108">Por padrão, essa operação (e as operações de tarefa POST, GET e [Complete](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="53026-108">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="53026-109">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="53026-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="53026-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="53026-110">Permissions</span></span>

<span data-ttu-id="53026-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53026-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53026-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53026-113">Permission type</span></span>      | <span data-ttu-id="53026-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53026-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53026-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53026-115">Delegated (work or school account)</span></span> | <span data-ttu-id="53026-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53026-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="53026-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53026-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53026-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53026-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="53026-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53026-119">Application</span></span> | <span data-ttu-id="53026-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53026-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53026-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53026-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53026-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53026-122">Request headers</span></span>

| <span data-ttu-id="53026-123">Nome</span><span class="sxs-lookup"><span data-stu-id="53026-123">Name</span></span>       | <span data-ttu-id="53026-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="53026-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="53026-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="53026-125">Authorization</span></span>  | <span data-ttu-id="53026-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53026-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53026-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="53026-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="53026-129">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="53026-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="53026-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="53026-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53026-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53026-131">Request body</span></span>

<span data-ttu-id="53026-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="53026-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="53026-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53026-135">Property</span></span> | <span data-ttu-id="53026-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="53026-136">Type</span></span> | <span data-ttu-id="53026-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="53026-137">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="53026-138">body</span><span class="sxs-lookup"><span data-stu-id="53026-138">body</span></span>|[<span data-ttu-id="53026-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="53026-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="53026-140">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-140">The task body that typically contains information about the task.</span></span> <span data-ttu-id="53026-141">Observe para qual tipo de HTML há suporte.</span><span class="sxs-lookup"><span data-stu-id="53026-141">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="53026-142">Categorias</span><span class="sxs-lookup"><span data-stu-id="53026-142">categories</span></span>|<span data-ttu-id="53026-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-143">String collection</span></span>|<span data-ttu-id="53026-144">As categorias associadas à postagem.</span><span class="sxs-lookup"><span data-stu-id="53026-144">The categories associated with the task.</span></span>|
|<span data-ttu-id="53026-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="53026-145">changeKey</span></span>|<span data-ttu-id="53026-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-146">String</span></span>|<span data-ttu-id="53026-147">A versão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-147">The version of the task.</span></span>|
|<span data-ttu-id="53026-148">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="53026-148">completedDateTime</span></span>|[<span data-ttu-id="53026-149">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53026-149">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="53026-150">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="53026-150">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="53026-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53026-151">createdDateTime</span></span>|<span data-ttu-id="53026-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53026-152">DateTimeOffset</span></span>|<span data-ttu-id="53026-153">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-153">The date and time when the task was created.</span></span> <span data-ttu-id="53026-154">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="53026-154">By default, it is in UTC.</span></span> <span data-ttu-id="53026-155">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53026-155">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="53026-156">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="53026-156">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="53026-157">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53026-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="53026-158">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="53026-158">dueDateTime</span></span>|[<span data-ttu-id="53026-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53026-159">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="53026-160">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="53026-160">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="53026-161">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="53026-161">hasAttachments</span></span>|<span data-ttu-id="53026-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="53026-162">Boolean</span></span>|<span data-ttu-id="53026-163">Defina como verdadeiro se a tarefa tiver anexos.</span><span class="sxs-lookup"><span data-stu-id="53026-163">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="53026-164">importância</span><span class="sxs-lookup"><span data-stu-id="53026-164">importance</span></span>|<span data-ttu-id="53026-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-165">string</span></span>|<span data-ttu-id="53026-166">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="53026-166">The importance of the event.</span></span> <span data-ttu-id="53026-167">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="53026-167">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="53026-168">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="53026-168">isReminderOn</span></span>|<span data-ttu-id="53026-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="53026-169">Boolean</span></span>|<span data-ttu-id="53026-170">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-170">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="53026-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53026-171">lastModifiedDateTime</span></span>|<span data-ttu-id="53026-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53026-172">DateTimeOffset</span></span>|<span data-ttu-id="53026-173">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-173">The date and time when the task was last modified.</span></span> <span data-ttu-id="53026-174">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="53026-174">By default, it is in UTC.</span></span> <span data-ttu-id="53026-175">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53026-175">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="53026-176">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="53026-176">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53026-177">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53026-177">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="53026-178">proprietário</span><span class="sxs-lookup"><span data-stu-id="53026-178">owner</span></span>|<span data-ttu-id="53026-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-179">String</span></span>|<span data-ttu-id="53026-180">O nome da pessoa que criou a tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-180">The name of the person who created the task.</span></span>|
|<span data-ttu-id="53026-181">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="53026-181">parentFolderId</span></span>|<span data-ttu-id="53026-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-182">String</span></span>|<span data-ttu-id="53026-183">O identificador exclusivo para a pasta pai da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-183">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="53026-184">recorrência</span><span class="sxs-lookup"><span data-stu-id="53026-184">recurrence</span></span>|[<span data-ttu-id="53026-185">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="53026-185">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="53026-186">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-186">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="53026-187">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="53026-187">reminderDateTime</span></span>|[<span data-ttu-id="53026-188">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53026-188">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="53026-189">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-189">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="53026-190">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="53026-190">sensitivity</span></span>|<span data-ttu-id="53026-191">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-191">string</span></span>|<span data-ttu-id="53026-192">Indica o nível de privacidade da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-192">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="53026-193">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="53026-193">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="53026-194">startDateTime</span><span class="sxs-lookup"><span data-stu-id="53026-194">startDateTime</span></span>|[<span data-ttu-id="53026-195">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="53026-195">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="53026-196">A data no fuso horário especificado que a tarefa será iniciada.</span><span class="sxs-lookup"><span data-stu-id="53026-196">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="53026-197">status</span><span class="sxs-lookup"><span data-stu-id="53026-197">status</span></span>|<span data-ttu-id="53026-198">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-198">string</span></span>|<span data-ttu-id="53026-199">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-199">Indicates the state or progress of the task.</span></span> <span data-ttu-id="53026-200">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="53026-200">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="53026-201">assunto</span><span class="sxs-lookup"><span data-stu-id="53026-201">subject</span></span>|<span data-ttu-id="53026-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53026-202">String</span></span>|<span data-ttu-id="53026-203">Uma breve descrição ou o título da tarefa.</span><span class="sxs-lookup"><span data-stu-id="53026-203">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="53026-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="53026-204">Response</span></span>

<span data-ttu-id="53026-205">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTask](../resources/outlooktask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53026-205">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53026-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53026-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="53026-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53026-207">Request</span></span>

<span data-ttu-id="53026-208">O exemplo a seguir modifica a propriedade **dueDateTime** e usa o `Prefer: outlook.timezone` cabeçalho para especificar a expressar as propriedades relacionadas à data na resposta na hora padrão do leste (EST).</span><span class="sxs-lookup"><span data-stu-id="53026-208">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="http"></a>[<span data-ttu-id="53026-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="53026-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="53026-210">C#</span><span class="sxs-lookup"><span data-stu-id="53026-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53026-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53026-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53026-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53026-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53026-213">Java</span><span class="sxs-lookup"><span data-stu-id="53026-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53026-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="53026-214">Response</span></span>

<span data-ttu-id="53026-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53026-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


