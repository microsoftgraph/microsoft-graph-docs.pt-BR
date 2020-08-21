---
title: Criar outlookTask
description: Criar uma tarefa do Outlook na pasta de tarefas especificada.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 862fc2374329396a818f668e677a15cbf3b0059c
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849342"
---
# <a name="create-outlooktask"></a><span data-ttu-id="e1f6b-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="e1f6b-103">Create outlookTask</span></span>

<span data-ttu-id="e1f6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="e1f6b-105">Criar uma tarefa do Outlook na pasta de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="e1f6b-106">O método POST sempre ignora a parte de hora de **StartDateTime** e **dueDateTime** no corpo da solicitação e pressupõe que o tempo seja sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1f6b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1f6b-107">Permissions</span></span>
<span data-ttu-id="e1f6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f6b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1f6b-110">Permission type</span></span>      | <span data-ttu-id="e1f6b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1f6b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1f6b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1f6b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e1f6b-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1f6b-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e1f6b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1f6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1f6b-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1f6b-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e1f6b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1f6b-116">Application</span></span> | <span data-ttu-id="e1f6b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1f6b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1f6b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="e1f6b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f6b-119">Request headers</span></span>
| <span data-ttu-id="e1f6b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e1f6b-120">Name</span></span>       | <span data-ttu-id="e1f6b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1f6b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1f6b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1f6b-122">Authorization</span></span>  | <span data-ttu-id="e1f6b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1f6b-125">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e1f6b-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e1f6b-126">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="e1f6b-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1f6b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f6b-128">Request body</span></span>
<span data-ttu-id="e1f6b-129">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="e1f6b-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1f6b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1f6b-130">Response</span></span>

<span data-ttu-id="e1f6b-131">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1f6b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1f6b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1f6b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f6b-133">Request</span></span>
<span data-ttu-id="e1f6b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
Content-type: application/json
Content-length: 376

{
  "subject": "Shop for dinner",
  "startDateTime": {
      "dateTime": "2016-04-23T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-04-25T13:00:00",
      "timeZone": "Pacific Standard Time"
  }
}
```
<span data-ttu-id="e1f6b-135">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="e1f6b-135">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1f6b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1f6b-136">Response</span></span>
<span data-ttu-id="e1f6b-137">O método POST ignora a parte da hora no corpo da solicitação e assume que a hora seja sempre meia-noite no fuso horário especificado (PST).</span><span class="sxs-lookup"><span data-stu-id="e1f6b-137">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="e1f6b-138">Em seguida, por padrão, o método POST converte e mostra todas as propriedades relacionadas à data em UTC na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-138">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="e1f6b-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1f6b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 376

{
  "createdDateTime": "2016-04-22T05:44:01.2012012Z",
  "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
  "categories": [ ],
  "assignedTo": "null",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-25T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments":false,
  "importance": "Normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTkAAAAIBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-04-23T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "NotStarted",
  "subject": "Shop for dinner"
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
  "suppressions": []
}
-->
