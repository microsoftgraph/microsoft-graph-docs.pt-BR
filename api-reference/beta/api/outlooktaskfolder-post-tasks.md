---
title: Criar outlookTask
description: Crie uma tarefa do Outlook na pasta tarefa especificada.
author: angelgolfer-ms
ms.openlocfilehash: 4d35c7de737e0de0f123dc9ee13f2f42e866d61d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322145"
---
# <a name="create-outlooktask"></a><span data-ttu-id="e7555-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="e7555-103">Create outlookTask</span></span>

> <span data-ttu-id="e7555-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7555-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7555-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7555-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7555-106">Crie uma tarefa do Outlook na pasta tarefa especificada.</span><span class="sxs-lookup"><span data-stu-id="e7555-106">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="e7555-107">O método POST sempre ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e supõe que o tempo para ser sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="e7555-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7555-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7555-108">Permissions</span></span>
<span data-ttu-id="e7555-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7555-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7555-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7555-111">Permission type</span></span>      | <span data-ttu-id="e7555-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7555-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7555-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7555-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e7555-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7555-114">Not supported.</span></span>    |
|<span data-ttu-id="e7555-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7555-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7555-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7555-116">Not supported.</span></span>    |
|<span data-ttu-id="e7555-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7555-117">Application</span></span> | <span data-ttu-id="e7555-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7555-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7555-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7555-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="e7555-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7555-120">Request headers</span></span>
| <span data-ttu-id="e7555-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e7555-121">Name</span></span>       | <span data-ttu-id="e7555-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7555-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7555-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7555-123">Authorization</span></span>  | <span data-ttu-id="e7555-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7555-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7555-126">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e7555-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e7555-127">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="e7555-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="e7555-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e7555-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7555-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7555-129">Request body</span></span>
<span data-ttu-id="e7555-130">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="e7555-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e7555-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7555-131">Response</span></span>

<span data-ttu-id="e7555-132">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7555-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7555-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7555-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7555-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7555-134">Request</span></span>
<span data-ttu-id="e7555-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7555-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="e7555-136">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="e7555-136">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e7555-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7555-137">Response</span></span>
<span data-ttu-id="e7555-138">O método POST ignora a parte da hora no corpo da solicitação e assume que a hora seja sempre meia-noite no fuso horário especificado (PST).</span><span class="sxs-lookup"><span data-stu-id="e7555-138">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="e7555-139">Em seguida, por padrão, o método POST converte e mostra todas as propriedades relacionadas à data em UTC na resposta.</span><span class="sxs-lookup"><span data-stu-id="e7555-139">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="e7555-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7555-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->