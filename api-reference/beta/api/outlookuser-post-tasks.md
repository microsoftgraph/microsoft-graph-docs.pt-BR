---
title: Criar outlookTask
description: Crie uma tarefa do Outlook no grupo de tarefas padrão`My Tasks`() e na pasta de`Tasks`tarefas padrão () na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f508aa05ad70246584ebc33bfaabc9317205011d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596085"
---
# <a name="create-outlooktask"></a><span data-ttu-id="aebaa-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="aebaa-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aebaa-104">Crie uma tarefa do Outlook no grupo de tarefas padrão`My Tasks`() e na pasta de`Tasks`tarefas padrão () na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="aebaa-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="aebaa-105">O método POST sempre ignora a parte de hora de **StartDateTime** e **dueDateTime** no corpo da solicitação e pressupõe que o tempo seja sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="aebaa-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="aebaa-106">Por padrão, essa operação (e o GET, PATCH e operações de tarefa [completa](../api/outlooktask-complete.md) ) retorna propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="aebaa-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="aebaa-107">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="aebaa-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="aebaa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="aebaa-108">Permissions</span></span>
<span data-ttu-id="aebaa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aebaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aebaa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aebaa-111">Permission type</span></span>      | <span data-ttu-id="aebaa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aebaa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aebaa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aebaa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aebaa-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aebaa-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="aebaa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aebaa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aebaa-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aebaa-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="aebaa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aebaa-117">Application</span></span> | <span data-ttu-id="aebaa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aebaa-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aebaa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aebaa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="aebaa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aebaa-120">Request headers</span></span>
| <span data-ttu-id="aebaa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="aebaa-121">Name</span></span>       | <span data-ttu-id="aebaa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aebaa-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aebaa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aebaa-123">Authorization</span></span>  | <span data-ttu-id="aebaa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aebaa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aebaa-126">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="aebaa-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="aebaa-127">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="aebaa-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="aebaa-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aebaa-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aebaa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aebaa-129">Request body</span></span>
<span data-ttu-id="aebaa-130">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="aebaa-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aebaa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aebaa-131">Response</span></span>

<span data-ttu-id="aebaa-132">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aebaa-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aebaa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aebaa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aebaa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aebaa-134">Request</span></span>
<span data-ttu-id="aebaa-135">O exemplo a seguir mostra o uso do `Prefer: outlook.timezone` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="aebaa-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="aebaa-136">Ele cria uma tarefa, expressa StartDateTime \*\*\*\* e **DueDateTime** na hora padrão do leste (EST) e inclui um `Prefer` cabeçalho do horário padrão do Pacífico (PST).</span><span class="sxs-lookup"><span data-stu-id="aebaa-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "assignedTo": "Dana Swope",
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
<span data-ttu-id="aebaa-137">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="aebaa-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aebaa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aebaa-138">Response</span></span>
<span data-ttu-id="aebaa-139">O método POST ignora a parte de hora de **StartDateTime** e **dueDateTime** no corpo da solicitação e pressupõe que o tempo seja sempre meia-noite no fuso horário especificado (EST).</span><span class="sxs-lookup"><span data-stu-id="aebaa-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="aebaa-140">Como o cabeçalho `Prefer` especifica PST, o método POST expressa todas as propriedades relacionadas à data na resposta em PST.</span><span class="sxs-lookup"><span data-stu-id="aebaa-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="aebaa-141">Em particular, para as \*\*\*\* Propriedades StartDateTime e **dueDateTime** , o método post converte meia-noite em est para pst e retorna-as em PST na resposta.</span><span class="sxs-lookup"><span data-stu-id="aebaa-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="aebaa-142">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="aebaa-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aebaa-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aebaa-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aebaa-144">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="aebaa-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aebaa-145">Basic</span><span class="sxs-lookup"><span data-stu-id="aebaa-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aebaa-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebaa-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
