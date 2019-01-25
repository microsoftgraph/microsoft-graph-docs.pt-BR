---
title: Criar outlookTask
description: Criar uma tarefa do Outlook no grupo de tarefa padrão (`My Tasks`) e a pasta de tarefas padrão (`Tasks`) na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 935732e14f7e467e3094d4a5a2f82d2922020569
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520988"
---
# <a name="create-outlooktask"></a><span data-ttu-id="2a4e3-103">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="2a4e3-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a4e3-104">Criar uma tarefa do Outlook no grupo de tarefa padrão (`My Tasks`) e a pasta de tarefas padrão (`Tasks`) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="2a4e3-105">O método POST sempre ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e supõe que o tempo para ser sempre meia-noite no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="2a4e3-106">Por padrão, esta operação (e as operações de tarefa GET, PATCH e [Concluir](../api/outlooktask-complete.md) ) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="2a4e3-107">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4e3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a4e3-108">Permissions</span></span>
<span data-ttu-id="2a4e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a4e3-111">Permission type</span></span>      | <span data-ttu-id="2a4e3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a4e3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a4e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a4e3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2a4e3-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a4e3-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2a4e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a4e3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4e3-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a4e3-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2a4e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a4e3-117">Application</span></span> | <span data-ttu-id="2a4e3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a4e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4e3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="2a4e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4e3-120">Request headers</span></span>
| <span data-ttu-id="2a4e3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2a4e3-121">Name</span></span>       | <span data-ttu-id="2a4e3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4e3-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a4e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a4e3-123">Authorization</span></span>  | <span data-ttu-id="2a4e3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a4e3-126">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2a4e3-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="2a4e3-127">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="2a4e3-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a4e3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4e3-129">Request body</span></span>
<span data-ttu-id="2a4e3-130">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="2a4e3-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2a4e3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4e3-131">Response</span></span>

<span data-ttu-id="2a4e3-132">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a4e3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a4e3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a4e3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4e3-134">Request</span></span>
<span data-ttu-id="2a4e3-135">O exemplo a seguir mostra o uso do `Prefer: outlook.timezone` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="2a4e3-136">Ele cria uma tarefa, expressa **startDateTime** e **dueDateTime** na hora padrão do Leste (EST) e inclui uma `Prefer` cabeçalho da hora oficial do Pacífico (PST).</span><span class="sxs-lookup"><span data-stu-id="2a4e3-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
<span data-ttu-id="2a4e3-137">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="2a4e3-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2a4e3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4e3-138">Response</span></span>
<span data-ttu-id="2a4e3-139">O método POST ignora a parte de tempo de **startDateTime** e **dueDateTime** no corpo da solicitação e supõe que o tempo para ser sempre meia-noite no fuso horário especificado (EST).</span><span class="sxs-lookup"><span data-stu-id="2a4e3-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="2a4e3-140">Como o cabeçalho `Prefer` especifica PST, o método POST expressa todas as propriedades relacionadas à data na resposta em PST.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="2a4e3-141">Em particular, para as propriedades **StartDateTime** e **DueDateTime**, o método POST converte meia-noite em EST para PST e os retorna em PST na resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="2a4e3-p107">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a4e3-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
