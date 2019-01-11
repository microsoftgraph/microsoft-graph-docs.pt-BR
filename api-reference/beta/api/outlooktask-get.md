---
title: Obter outlookTask
description: Obtenha as propriedades e relacionamentos de uma tarefa do Outlook na caixa de correio do usuário.
localization_priority: Normal
ms.openlocfilehash: f93bc46a1bbe3f7a6c145458606174b6e3a13f1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822222"
---
# <a name="get-outlooktask"></a><span data-ttu-id="5d15c-103">Obter outlookTask</span><span class="sxs-lookup"><span data-stu-id="5d15c-103">Get outlookTask</span></span>

> <span data-ttu-id="5d15c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d15c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d15c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d15c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d15c-106">Obtenha as propriedades e relacionamentos de uma tarefa do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d15c-106">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="5d15c-107">Por padrão, esta operação (e as operações de tarefa POST, PATCH e [Concluir](../api/outlooktask-complete.md) ) retorna propriedades relacionadas a data em UTC.</span><span class="sxs-lookup"><span data-stu-id="5d15c-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="5d15c-108">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="5d15c-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d15c-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="5d15c-109">Permissions</span></span>

<span data-ttu-id="5d15c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d15c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d15c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d15c-112">Permission type</span></span>      | <span data-ttu-id="5d15c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d15c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d15c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d15c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5d15c-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5d15c-115">Tasks.Read</span></span>    |
|<span data-ttu-id="5d15c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d15c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d15c-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5d15c-117">Tasks.Read</span></span>    |
|<span data-ttu-id="5d15c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d15c-118">Application</span></span> | <span data-ttu-id="5d15c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d15c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d15c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d15c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d15c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d15c-121">Optional query parameters</span></span>

<span data-ttu-id="5d15c-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d15c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d15c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d15c-123">Request headers</span></span>

| <span data-ttu-id="5d15c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5d15c-124">Name</span></span>      |<span data-ttu-id="5d15c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d15c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d15c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d15c-126">Authorization</span></span>  | <span data-ttu-id="5d15c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d15c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d15c-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5d15c-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="5d15c-130">Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="5d15c-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="5d15c-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d15c-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d15c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d15c-132">Request body</span></span>

<span data-ttu-id="5d15c-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d15c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d15c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d15c-134">Response</span></span>

<span data-ttu-id="5d15c-135">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d15c-135">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="5d15c-136">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="5d15c-136">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="5d15c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d15c-137">Request</span></span>

<span data-ttu-id="5d15c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d15c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

### <a name="response"></a><span data-ttu-id="5d15c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d15c-139">Response</span></span>

<span data-ttu-id="5d15c-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d15c-140">Here is an example of the response.</span></span> <span data-ttu-id="5d15c-141">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="5d15c-141">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="5d15c-142">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5d15c-142">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d15c-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d15c-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [ ],
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
  "hasAttachments":false,
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

## <a name="example-2"></a><span data-ttu-id="5d15c-144">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="5d15c-144">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="5d15c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d15c-145">Request</span></span>

<span data-ttu-id="5d15c-146">Este exemplo usa o `Prefer: outlook.timezone` cabeçalho para especificar a exibição de propriedades de data / hora na resposta na hora oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="5d15c-146">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="5d15c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d15c-147">Response</span></span>

<span data-ttu-id="5d15c-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d15c-148">Here is an example of the response.</span></span> <span data-ttu-id="5d15c-149">As propriedades de data / hora na resposta são exibidas na hora oficial do Pacífico especificada.</span><span class="sxs-lookup"><span data-stu-id="5d15c-149">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="5d15c-150">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5d15c-150">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d15c-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d15c-151">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
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
    "contentType": "text",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
