---
title: Listar tarefas
description: Obtenha todas as tarefas do Outlook na caixa de correio do usuário.
ms.openlocfilehash: df295b40b0813813733b61c2a09b53903cce0d79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035361"
---
# <a name="list-tasks"></a><span data-ttu-id="5d07e-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="5d07e-103">List tasks</span></span>

> <span data-ttu-id="5d07e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d07e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d07e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d07e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d07e-106">Obtenha todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d07e-106">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="5d07e-107">Por padrão, esta operação (e as operações de tarefa POST, PATCH e [Concluir](../api/outlooktask-complete.md) ) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="5d07e-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="5d07e-108">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="5d07e-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="5d07e-109">Ver um [exemplo](outlooktask-get.md#example-2) para obter uma única tarefa.</span><span class="sxs-lookup"><span data-stu-id="5d07e-109">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="5d07e-110">Você pode aplicar o cabeçalho da mesma forma para obter várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="5d07e-110">You can apply the header similarly to get multiple tasks.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5d07e-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="5d07e-111">Permissions</span></span>
<span data-ttu-id="5d07e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d07e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d07e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d07e-114">Permission type</span></span>      | <span data-ttu-id="5d07e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d07e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d07e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d07e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5d07e-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5d07e-117">Tasks.Read</span></span>    |
|<span data-ttu-id="5d07e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d07e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d07e-119">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5d07e-119">Tasks.Read</span></span>    |
|<span data-ttu-id="5d07e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d07e-120">Application</span></span> | <span data-ttu-id="5d07e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d07e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d07e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d07e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d07e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d07e-123">Optional query parameters</span></span>
<span data-ttu-id="5d07e-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d07e-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d07e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d07e-125">Request headers</span></span>
| <span data-ttu-id="5d07e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="5d07e-126">Name</span></span>      |<span data-ttu-id="5d07e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d07e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d07e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d07e-128">Authorization</span></span>  | <span data-ttu-id="5d07e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d07e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d07e-131">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5d07e-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="5d07e-132">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="5d07e-132">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="5d07e-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d07e-133">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d07e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d07e-134">Request body</span></span>
<span data-ttu-id="5d07e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d07e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d07e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d07e-136">Response</span></span>

<span data-ttu-id="5d07e-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d07e-137">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d07e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d07e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d07e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d07e-139">Request</span></span>
<span data-ttu-id="5d07e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d07e-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
##### <a name="response"></a><span data-ttu-id="5d07e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d07e-141">Response</span></span>
<span data-ttu-id="5d07e-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d07e-142">Here is an example of the response.</span></span> <span data-ttu-id="5d07e-143">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="5d07e-143">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="5d07e-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d07e-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
   {
      "id": "AAMkADA1MTrfAAA=",
      "createdDateTime": "2016-04-22T05:44:01.2012012Z",
      "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-25T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-23T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    },
    {
      "id": "AAMkADA1MTrgAAA=",
      "createdDateTime": "2016-04-22T06:03:35.9279794Z",
      "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-27T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-26T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->