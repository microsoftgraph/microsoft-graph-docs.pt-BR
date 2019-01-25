---
title: Criar outlookTask
description: Crie uma tarefa do Outlook na pasta tarefa especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8ba293d83e2a202a45cfebf4c318ee73d808e1e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510593"
---
# <a name="create-outlooktask"></a><span data-ttu-id="ad6de-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="ad6de-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad6de-104">Crie uma tarefa do Outlook na pasta tarefa especificada.</span><span class="sxs-lookup"><span data-stu-id="ad6de-104">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="ad6de-105">O método POST sempre ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e supõe que o tempo para ser sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="ad6de-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad6de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad6de-106">Permissions</span></span>
<span data-ttu-id="ad6de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad6de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad6de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad6de-109">Permission type</span></span>      | <span data-ttu-id="ad6de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad6de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad6de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad6de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad6de-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad6de-112">Not supported.</span></span>    |
|<span data-ttu-id="ad6de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad6de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad6de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad6de-114">Not supported.</span></span>    |
|<span data-ttu-id="ad6de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad6de-115">Application</span></span> | <span data-ttu-id="ad6de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad6de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad6de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad6de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="ad6de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad6de-118">Request headers</span></span>
| <span data-ttu-id="ad6de-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ad6de-119">Name</span></span>       | <span data-ttu-id="ad6de-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad6de-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad6de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad6de-121">Authorization</span></span>  | <span data-ttu-id="ad6de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad6de-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad6de-124">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ad6de-124">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ad6de-125">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="ad6de-125">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="ad6de-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad6de-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad6de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad6de-127">Request body</span></span>
<span data-ttu-id="ad6de-128">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="ad6de-128">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad6de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad6de-129">Response</span></span>

<span data-ttu-id="ad6de-130">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad6de-130">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad6de-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad6de-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad6de-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad6de-132">Request</span></span>
<span data-ttu-id="ad6de-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad6de-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="ad6de-134">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="ad6de-134">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ad6de-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad6de-135">Response</span></span>
<span data-ttu-id="ad6de-136">O método POST ignora a parte da hora no corpo da solicitação e assume que a hora seja sempre meia-noite no fuso horário especificado (PST).</span><span class="sxs-lookup"><span data-stu-id="ad6de-136">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="ad6de-137">Em seguida, por padrão, o método POST converte e mostra todas as propriedades relacionadas à data em UTC na resposta.</span><span class="sxs-lookup"><span data-stu-id="ad6de-137">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="ad6de-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad6de-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
