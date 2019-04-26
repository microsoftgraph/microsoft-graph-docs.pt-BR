---
title: Criar outlookTask
description: Criar uma tarefa do Outlook na pasta de tarefas especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 050d45319f822531c951a665788f1c1669406532
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337898"
---
# <a name="create-outlooktask"></a><span data-ttu-id="9b564-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="9b564-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b564-104">Criar uma tarefa do Outlook na pasta de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="9b564-104">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="9b564-105">O método POST sempre ignora a parte de hora de **StartDateTime** e **dueDateTime** no corpo da solicitação e pressupõe que o tempo seja sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="9b564-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b564-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b564-106">Permissions</span></span>
<span data-ttu-id="9b564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b564-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b564-109">Permission type</span></span>      | <span data-ttu-id="9b564-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b564-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b564-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b564-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b564-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b564-112">Not supported.</span></span>    |
|<span data-ttu-id="9b564-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b564-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b564-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b564-114">Not supported.</span></span>    |
|<span data-ttu-id="9b564-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b564-115">Application</span></span> | <span data-ttu-id="9b564-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b564-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b564-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b564-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="9b564-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b564-118">Request headers</span></span>
| <span data-ttu-id="9b564-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9b564-119">Name</span></span>       | <span data-ttu-id="9b564-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b564-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b564-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b564-121">Authorization</span></span>  | <span data-ttu-id="9b564-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b564-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b564-124">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9b564-124">Prefer: outlook.timezone</span></span> | <span data-ttu-id="9b564-125">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="9b564-125">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="9b564-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9b564-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b564-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b564-127">Request body</span></span>
<span data-ttu-id="9b564-128">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="9b564-128">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9b564-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b564-129">Response</span></span>

<span data-ttu-id="9b564-130">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b564-130">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b564-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b564-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b564-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b564-132">Request</span></span>
<span data-ttu-id="9b564-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b564-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="9b564-134">No corpo da solicitação, forneça uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="9b564-134">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9b564-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b564-135">Response</span></span>
<span data-ttu-id="9b564-136">O método POST ignora a parte da hora no corpo da solicitação e assume que a hora seja sempre meia-noite no fuso horário especificado (PST).</span><span class="sxs-lookup"><span data-stu-id="9b564-136">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="9b564-137">Em seguida, por padrão, o método POST converte e mostra todas as propriedades relacionadas à data em UTC na resposta.</span><span class="sxs-lookup"><span data-stu-id="9b564-137">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="9b564-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b564-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
