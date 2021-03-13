---
title: Criar outlookTask
description: Crie uma tarefa do Outlook na pasta de tarefas especificada.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5986d4fe2ab77cf8c4634f3d872d966819ebca7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774303"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="98561-103">Criar outlookTask(obsoleto)</span><span class="sxs-lookup"><span data-stu-id="98561-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="98561-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98561-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="98561-105">Crie uma tarefa do Outlook na pasta de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="98561-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="98561-106">O método POST sempre ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e assume o tempo para ser sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="98561-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="98561-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="98561-107">Permissions</span></span>
<span data-ttu-id="98561-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98561-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98561-110">Permission type</span></span>      | <span data-ttu-id="98561-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98561-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98561-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98561-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98561-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98561-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="98561-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98561-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98561-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98561-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="98561-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98561-116">Application</span></span> | <span data-ttu-id="98561-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98561-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98561-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98561-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="98561-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98561-119">Request headers</span></span>
| <span data-ttu-id="98561-120">Nome</span><span class="sxs-lookup"><span data-stu-id="98561-120">Name</span></span>       | <span data-ttu-id="98561-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="98561-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98561-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98561-122">Authorization</span></span>  | <span data-ttu-id="98561-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98561-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98561-125">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="98561-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="98561-126">Especifica o fuso horário para propriedades de tempo na resposta, que estaria em UTC se esse header não for especificado.</span><span class="sxs-lookup"><span data-stu-id="98561-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="98561-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="98561-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98561-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98561-128">Request body</span></span>
<span data-ttu-id="98561-129">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="98561-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98561-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="98561-130">Response</span></span>

<span data-ttu-id="98561-131">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98561-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98561-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98561-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98561-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98561-133">Request</span></span>
<span data-ttu-id="98561-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98561-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98561-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="98561-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
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
# <a name="c"></a>[<span data-ttu-id="98561-136">C#</span><span class="sxs-lookup"><span data-stu-id="98561-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98561-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98561-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98561-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98561-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98561-139">Java</span><span class="sxs-lookup"><span data-stu-id="98561-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktask-from-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="98561-140">No corpo da solicitação, fornece uma representação JSON do [objeto outlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="98561-140">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="98561-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="98561-141">Response</span></span>
<span data-ttu-id="98561-142">O método POST ignora a parte da hora no corpo da solicitação e assume que a hora seja sempre meia-noite no fuso horário especificado (PST).</span><span class="sxs-lookup"><span data-stu-id="98561-142">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="98561-143">Em seguida, por padrão, o método POST converte e mostra todas as propriedades relacionadas à data em UTC na resposta.</span><span class="sxs-lookup"><span data-stu-id="98561-143">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="98561-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98561-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


