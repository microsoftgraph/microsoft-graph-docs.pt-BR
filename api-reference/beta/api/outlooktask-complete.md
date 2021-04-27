---
title: 'outlookTask: concluído'
description: 'Conclua uma Outlook que define a **propriedade completedDateTime** como a data atual, '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 35ff88db1fb8cde5c84a6010fc6e33b81661c387
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055481"
---
# <a name="outlooktask-complete-deprecated"></a><span data-ttu-id="8fbc8-103">outlookTask: completo (preterido)</span><span class="sxs-lookup"><span data-stu-id="8fbc8-103">outlookTask: complete (deprecated)</span></span>

<span data-ttu-id="8fbc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fbc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="8fbc8-105">Conclua uma Outlook que define a propriedade **completedDateTime** como a data atual e a **propriedade status** como `completed` .</span><span class="sxs-lookup"><span data-stu-id="8fbc8-105">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="8fbc8-106">Se você estiver concluindo uma tarefa em uma série recorrente, na resposta, a coleção de tarefas conterá a tarefa concluída na série e a próxima tarefa na série.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-106">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="8fbc8-107">A **propriedade completedDateTime** representa a data em que a tarefa é concluída.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-107">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="8fbc8-108">A parte de tempo **de completedDateTime** é definida como UTC meia-noite por padrão.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-108">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="8fbc8-109">Por padrão, essa operação (e as operações de tarefa POST, GET e PATCH) retorna propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-109">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="8fbc8-110">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fbc8-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fbc8-111">Permissions</span></span>

<span data-ttu-id="8fbc8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fbc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fbc8-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fbc8-114">Permission type</span></span>      | <span data-ttu-id="8fbc8-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fbc8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fbc8-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fbc8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8fbc8-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fbc8-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8fbc8-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fbc8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fbc8-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fbc8-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8fbc8-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fbc8-120">Application</span></span> | <span data-ttu-id="8fbc8-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fbc8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fbc8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="8fbc8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbc8-123">Request headers</span></span>

| <span data-ttu-id="8fbc8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8fbc8-124">Name</span></span>       | <span data-ttu-id="8fbc8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fbc8-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8fbc8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fbc8-126">Authorization</span></span>  | <span data-ttu-id="8fbc8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8fbc8-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8fbc8-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8fbc8-130">Especifica o fuso horário para propriedades de tempo na resposta, que estaria em UTC se esse header não for especificado.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8fbc8-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fbc8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbc8-132">Request body</span></span>

<span data-ttu-id="8fbc8-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fbc8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fbc8-134">Response</span></span>

<span data-ttu-id="8fbc8-135">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-135">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fbc8-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fbc8-136">Example</span></span>

<span data-ttu-id="8fbc8-137">O exemplo a seguir marca a tarefa especificada como concluída.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="8fbc8-138">Especifica o Horário Padrão do Pacífico (PST) no `Prefer: outlook.timezone` header.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="8fbc8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbc8-139">Request</span></span>

<span data-ttu-id="8fbc8-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8fbc8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fbc8-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="8fbc8-142">C#</span><span class="sxs-lookup"><span data-stu-id="8fbc8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlooktask-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fbc8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fbc8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlooktask-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fbc8-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fbc8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlooktask-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8fbc8-145">Java</span><span class="sxs-lookup"><span data-stu-id="8fbc8-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlooktask-complete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8fbc8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fbc8-146">Response</span></span>

<span data-ttu-id="8fbc8-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-147">Here is an example of the response.</span></span> <span data-ttu-id="8fbc8-148">As **propriedades completedDateTime** e outras relacionadas à data na resposta são expressas em PST.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-148">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="8fbc8-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8fbc8-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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


