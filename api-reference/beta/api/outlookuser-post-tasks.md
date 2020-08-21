---
title: Criar outlookTask
description: Crie uma tarefa do Outlook no grupo de tarefas padrão ( `My Tasks` ) e na pasta de tarefas padrão ( `Tasks` ) na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8de61bceba328dbf99242cbfe5140e7ebed1296b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849447"
---
# <a name="create-outlooktask"></a><span data-ttu-id="9742c-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="9742c-103">Create outlookTask</span></span>

<span data-ttu-id="9742c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9742c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="9742c-105">Crie uma tarefa do Outlook no grupo de tarefas padrão ( `My Tasks` ) e na pasta de tarefas padrão ( `Tasks` ) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9742c-105">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="9742c-106">O método POST sempre ignora a parte de hora de **StartDateTime** e **dueDateTime** no corpo da solicitação e pressupõe que o tempo seja sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="9742c-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="9742c-107">Por padrão, essa operação (e o GET, PATCH e operações de tarefa [completa](../api/outlooktask-complete.md) ) retorna propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="9742c-107">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="9742c-108">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="9742c-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="9742c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9742c-109">Permissions</span></span>
<span data-ttu-id="9742c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9742c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9742c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9742c-112">Permission type</span></span>      | <span data-ttu-id="9742c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9742c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9742c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9742c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9742c-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9742c-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9742c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9742c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9742c-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9742c-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9742c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9742c-118">Application</span></span> | <span data-ttu-id="9742c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9742c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9742c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9742c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="9742c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9742c-121">Request headers</span></span>
| <span data-ttu-id="9742c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9742c-122">Name</span></span>       | <span data-ttu-id="9742c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9742c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9742c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9742c-124">Authorization</span></span>  | <span data-ttu-id="9742c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9742c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9742c-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9742c-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="9742c-128">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="9742c-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="9742c-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9742c-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9742c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9742c-130">Request body</span></span>
<span data-ttu-id="9742c-131">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="9742c-131">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9742c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9742c-132">Response</span></span>

<span data-ttu-id="9742c-133">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9742c-133">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9742c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9742c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9742c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9742c-135">Request</span></span>
<span data-ttu-id="9742c-136">O exemplo a seguir mostra o uso do `Prefer: outlook.timezone` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="9742c-136">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="9742c-137">Ele cria uma tarefa, expressa **StartDateTime** e **DueDateTime** na hora padrão do leste (EST) e inclui um `Prefer` cabeçalho do horário padrão do Pacífico (PST).</span><span class="sxs-lookup"><span data-stu-id="9742c-137">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
# <a name="c"></a>[<span data-ttu-id="9742c-138">C#</span><span class="sxs-lookup"><span data-stu-id="9742c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9742c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9742c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9742c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9742c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9742c-141">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="9742c-141">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9742c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9742c-142">Response</span></span>
<span data-ttu-id="9742c-143">O método POST ignora a parte de hora de **StartDateTime** e **dueDateTime** no corpo da solicitação e pressupõe que o tempo seja sempre meia-noite no fuso horário especificado (EST).</span><span class="sxs-lookup"><span data-stu-id="9742c-143">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="9742c-144">Como o cabeçalho `Prefer` especifica PST, o método POST expressa todas as propriedades relacionadas à data na resposta em PST.</span><span class="sxs-lookup"><span data-stu-id="9742c-144">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="9742c-145">Em particular, para as propriedades **StartDateTime** e **dueDateTime** , o método post converte meia-noite em est para pst e retorna-as em PST na resposta.</span><span class="sxs-lookup"><span data-stu-id="9742c-145">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="9742c-p107">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9742c-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "assignedTo": null,
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
  ]
}
-->
