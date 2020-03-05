---
title: 'outlookTask: concluir'
description: 'Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** para a data atual, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: afe7f34d634a52c369916ca5acc68c05a1b6030c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456184"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="b68a6-103">outlookTask: concluir</span><span class="sxs-lookup"><span data-stu-id="b68a6-103">outlookTask: complete</span></span>

<span data-ttu-id="b68a6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b68a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b68a6-105">Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** como a data atual e a propriedade **status** como `completed`.</span><span class="sxs-lookup"><span data-stu-id="b68a6-105">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="b68a6-106">Se você estiver realizando uma tarefa em uma série recorrente, na resposta, a coleção de tarefas conterá a tarefa concluída na série e a próxima tarefa na série.</span><span class="sxs-lookup"><span data-stu-id="b68a6-106">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="b68a6-107">A propriedade **completedDateTime** representa a data em que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="b68a6-107">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="b68a6-108">A parte de hora de **completedDateTime** é definida como meia-noite UTC por padrão.</span><span class="sxs-lookup"><span data-stu-id="b68a6-108">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="b68a6-109">Por padrão, essa operação (e as operações de tarefa POST, GET e PATCH) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="b68a6-109">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="b68a6-110">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="b68a6-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="b68a6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b68a6-111">Permissions</span></span>

<span data-ttu-id="b68a6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b68a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b68a6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b68a6-114">Permission type</span></span>      | <span data-ttu-id="b68a6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b68a6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b68a6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b68a6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b68a6-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b68a6-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b68a6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b68a6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b68a6-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b68a6-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b68a6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b68a6-120">Application</span></span> | <span data-ttu-id="b68a6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b68a6-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b68a6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b68a6-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="b68a6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b68a6-123">Request headers</span></span>

| <span data-ttu-id="b68a6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b68a6-124">Name</span></span>       | <span data-ttu-id="b68a6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b68a6-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b68a6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b68a6-126">Authorization</span></span>  | <span data-ttu-id="b68a6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b68a6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b68a6-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b68a6-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="b68a6-130">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="b68a6-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="b68a6-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b68a6-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b68a6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b68a6-132">Request body</span></span>

<span data-ttu-id="b68a6-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b68a6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b68a6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b68a6-134">Response</span></span>

<span data-ttu-id="b68a6-135">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b68a6-135">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b68a6-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b68a6-136">Example</span></span>

<span data-ttu-id="b68a6-137">O exemplo a seguir marca a tarefa especificada como concluída.</span><span class="sxs-lookup"><span data-stu-id="b68a6-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="b68a6-138">Ele especifica o `Prefer: outlook.timezone` horário padrão do Pacífico (PST) no cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="b68a6-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="b68a6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b68a6-139">Request</span></span>

<span data-ttu-id="b68a6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b68a6-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="b68a6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b68a6-141">Response</span></span>

<span data-ttu-id="b68a6-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b68a6-142">Here is an example of the response.</span></span> <span data-ttu-id="b68a6-143">A **completedDateTime** e outras propriedades relacionadas à data na resposta são expressas em PST.</span><span class="sxs-lookup"><span data-stu-id="b68a6-143">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="b68a6-144">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b68a6-144">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b68a6-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b68a6-145">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
