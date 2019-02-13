---
title: Obter outlookTask
description: Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f140734b6e5fa3e6488b71dbe183a9e3d82fc795
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967288"
---
# <a name="get-outlooktask"></a><span data-ttu-id="c3936-103">Obter outlookTask</span><span class="sxs-lookup"><span data-stu-id="c3936-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3936-104">Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3936-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="c3936-105">Por padrão, esta operação (e as operações de tarefa POST, PATCH e [Concluir](../api/outlooktask-complete.md) ) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="c3936-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="c3936-106">Você pode usar o `Prefer: outlook.timezone` cabeçalho para que todas as propriedades relacionadas às datas como resposta representada em um fuso horário diferente do UTC.</span><span class="sxs-lookup"><span data-stu-id="c3936-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3936-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3936-107">Permissions</span></span>

<span data-ttu-id="c3936-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3936-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3936-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3936-110">Permission type</span></span>                        | <span data-ttu-id="c3936-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3936-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="c3936-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3936-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3936-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c3936-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="c3936-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3936-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3936-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c3936-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="c3936-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3936-116">Application</span></span>                            | <span data-ttu-id="c3936-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3936-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="c3936-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3936-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3936-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3936-119">Optional query parameters</span></span>

<span data-ttu-id="c3936-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c3936-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3936-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3936-121">Request headers</span></span>

| <span data-ttu-id="c3936-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c3936-122">Name</span></span>                     | <span data-ttu-id="c3936-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3936-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="c3936-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3936-124">Authorization</span></span>            | <span data-ttu-id="c3936-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3936-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="c3936-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c3936-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c3936-128">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="c3936-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c3936-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3936-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3936-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3936-130">Request body</span></span>

<span data-ttu-id="c3936-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3936-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3936-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3936-132">Response</span></span>

<span data-ttu-id="c3936-133">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3936-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3936-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3936-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="c3936-135">O exemplo 1: Obtenha uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="c3936-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="c3936-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3936-136">Request</span></span>

<span data-ttu-id="c3936-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3936-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c3936-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3936-138">Response</span></span>

<span data-ttu-id="c3936-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3936-139">Here is an example of the response.</span></span> <span data-ttu-id="c3936-140">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="c3936-140">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="c3936-141">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c3936-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c3936-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3936-142">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
  "assignedTo": null,
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-27T04:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-04-26T04:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "notStarted",
  "subject": "Shop for dinner"
}
```

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="c3936-143">Exemplo 2: Obter tarefa do Outlook com as propriedades de data / hora em hora oficial do Pacífico</span><span class="sxs-lookup"><span data-stu-id="c3936-143">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="c3936-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3936-144">Request</span></span>

<span data-ttu-id="c3936-145">Este exemplo usa o `Prefer: outlook.timezone` cabeçalho para especificar que a API deve retornar as propriedades de data / hora na resposta na hora oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="c3936-145">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="c3936-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3936-146">Response</span></span>

<span data-ttu-id="c3936-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3936-147">Here is an example of the response.</span></span> <span data-ttu-id="c3936-148">As propriedades de data / hora na resposta são retornadas na hora oficial do Pacífico especificada.</span><span class="sxs-lookup"><span data-stu-id="c3936-148">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="c3936-149">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c3936-149">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c3936-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3936-150">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
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
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
