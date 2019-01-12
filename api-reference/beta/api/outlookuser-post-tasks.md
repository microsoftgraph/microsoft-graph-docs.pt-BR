---
title: Criar outlookTask
description: Criar uma tarefa do Outlook no grupo de tarefa padrão (`My Tasks`) e a pasta de tarefas padrão (`Tasks`) na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 04cc91f9c6eee09f71783d0548470d167911ec91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925592"
---
# <a name="create-outlooktask"></a><span data-ttu-id="3db27-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="3db27-103">Create outlookTask</span></span>

> <span data-ttu-id="3db27-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3db27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3db27-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3db27-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3db27-106">Criar uma tarefa do Outlook no grupo de tarefa padrão (`My Tasks`) e a pasta de tarefas padrão (`Tasks`) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3db27-106">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="3db27-107">O método POST sempre ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e supõe que o tempo para ser sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="3db27-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="3db27-108">Por padrão, esta operação (e as operações de tarefa GET, PATCH e [Concluir](../api/outlooktask-complete.md) ) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="3db27-108">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="3db27-109">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="3db27-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="3db27-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="3db27-110">Permissions</span></span>
<span data-ttu-id="3db27-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db27-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3db27-113">Permission type</span></span>      | <span data-ttu-id="3db27-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3db27-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db27-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3db27-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3db27-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db27-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3db27-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3db27-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db27-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db27-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3db27-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3db27-119">Application</span></span> | <span data-ttu-id="3db27-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3db27-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3db27-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3db27-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="3db27-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3db27-122">Request headers</span></span>
| <span data-ttu-id="3db27-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3db27-123">Name</span></span>       | <span data-ttu-id="3db27-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3db27-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3db27-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3db27-125">Authorization</span></span>  | <span data-ttu-id="3db27-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3db27-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3db27-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3db27-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="3db27-129">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="3db27-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="3db27-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3db27-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3db27-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3db27-131">Request body</span></span>
<span data-ttu-id="3db27-132">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="3db27-132">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3db27-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3db27-133">Response</span></span>

<span data-ttu-id="3db27-134">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3db27-134">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3db27-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3db27-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3db27-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3db27-136">Request</span></span>
<span data-ttu-id="3db27-137">O exemplo a seguir mostra o uso do `Prefer: outlook.timezone` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="3db27-137">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="3db27-138">Ele cria uma tarefa, expressa **startDateTime** e **dueDateTime** na hora padrão do Leste (EST) e inclui uma `Prefer` cabeçalho da hora oficial do Pacífico (PST).</span><span class="sxs-lookup"><span data-stu-id="3db27-138">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
<span data-ttu-id="3db27-139">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="3db27-139">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3db27-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3db27-140">Response</span></span>
<span data-ttu-id="3db27-141">O método POST ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e supõe que o tempo para ser sempre meia-noite no fuso horário especificado (EST).</span><span class="sxs-lookup"><span data-stu-id="3db27-141">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="3db27-142">Como o cabeçalho `Prefer` especifica PST, o método POST expressa todas as propriedades relacionadas à data na resposta em PST.</span><span class="sxs-lookup"><span data-stu-id="3db27-142">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="3db27-143">Em particular, para as propriedades **startDateTime** e **dueDateTime** , o método POST converte meia-noite no EST para PST e os retorna em PST na resposta.</span><span class="sxs-lookup"><span data-stu-id="3db27-143">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="3db27-p108">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3db27-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
