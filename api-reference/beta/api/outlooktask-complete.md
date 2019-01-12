---
title: 'outlookTask: completa'
description: 'Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** como a data atual, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 966f5c2a6d429169cff3bd6746ebb0bace34ad15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979632"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="41b4e-103">outlookTask: completa</span><span class="sxs-lookup"><span data-stu-id="41b4e-103">outlookTask: complete</span></span>

> <span data-ttu-id="41b4e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41b4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41b4e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41b4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41b4e-106">Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** como a data atual e a propriedade **status** para `completed`.</span><span class="sxs-lookup"><span data-stu-id="41b4e-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="41b4e-107">Se estiver Concluindo uma tarefa em uma série recorrente, na resposta, a coleção de tarefa conterá tarefa concluída na série e a próxima tarefa na série.</span><span class="sxs-lookup"><span data-stu-id="41b4e-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="41b4e-108">A propriedade **completedDateTime** representa a data quando a tarefa é concluída.</span><span class="sxs-lookup"><span data-stu-id="41b4e-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="41b4e-109">Por padrão, a parte do tempo de **completedDateTime** é definida como meia-noite UTC.</span><span class="sxs-lookup"><span data-stu-id="41b4e-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="41b4e-110">Por padrão, esta operação (e as operações de tarefa POST, GET e PATCH) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="41b4e-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="41b4e-111">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="41b4e-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="41b4e-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="41b4e-112">Permissions</span></span>

<span data-ttu-id="41b4e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41b4e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b4e-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41b4e-115">Permission type</span></span>      | <span data-ttu-id="41b4e-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41b4e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41b4e-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41b4e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="41b4e-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41b4e-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="41b4e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41b4e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41b4e-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41b4e-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="41b4e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41b4e-121">Application</span></span> | <span data-ttu-id="41b4e-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41b4e-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41b4e-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41b4e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="41b4e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41b4e-124">Request headers</span></span>

| <span data-ttu-id="41b4e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="41b4e-125">Name</span></span>       | <span data-ttu-id="41b4e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b4e-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41b4e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="41b4e-127">Authorization</span></span>  | <span data-ttu-id="41b4e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41b4e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41b4e-130">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="41b4e-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="41b4e-131">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="41b4e-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="41b4e-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="41b4e-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41b4e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41b4e-133">Request body</span></span>

<span data-ttu-id="41b4e-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41b4e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41b4e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b4e-135">Response</span></span>

<span data-ttu-id="41b4e-136">Se tiver êxito, este método retornará `200 OK` código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41b4e-136">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41b4e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41b4e-137">Example</span></span>

<span data-ttu-id="41b4e-138">O exemplo a seguir marca a tarefa especificada como concluída.</span><span class="sxs-lookup"><span data-stu-id="41b4e-138">The following example marks the specified task as complete.</span></span> <span data-ttu-id="41b4e-139">Hora oficial do Pacífico (PST) em Especifica o `Prefer: outlook.timezone` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="41b4e-139">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="41b4e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41b4e-140">Request</span></span>

<span data-ttu-id="41b4e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41b4e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="41b4e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b4e-142">Response</span></span>

<span data-ttu-id="41b4e-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41b4e-143">Here is an example of the response.</span></span> <span data-ttu-id="41b4e-144">O **completedDateTime** e outras propriedades relacionadas a data na resposta são expressos em PST.</span><span class="sxs-lookup"><span data-stu-id="41b4e-144">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="41b4e-145">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="41b4e-145">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="41b4e-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41b4e-146">All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
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
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
