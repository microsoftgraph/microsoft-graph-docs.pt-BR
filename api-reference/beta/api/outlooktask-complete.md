---
title: 'outlookTask: concluído'
description: 'Conclua uma tarefa do Outlook que define a **propriedade completedDateTime** como a data atual, '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: edf7f24efc2a3c208a1aed4c4a03e41ad596c4c4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471842"
---
# <a name="outlooktask-complete-deprecated"></a>outlookTask: completo (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Conclua uma tarefa do Outlook que define a **propriedade completedDateTime** como a data atual e a **propriedade status** como `completed` .

Se você estiver concluindo uma tarefa em uma série recorrente, na resposta, a coleção de tarefas conterá a tarefa concluída na série e a próxima tarefa na série.

A **propriedade completedDateTime** representa a data em que a tarefa é concluída. A parte de tempo **de completedDateTime** é definida como UTC meia-noite por padrão.

Por padrão, essa operação (e as operações de tarefa POST, GET e PATCH) retorna propriedades relacionadas à data em UTC. Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Tasks.ReadWrite    |
|Delegada (conta pessoal da Microsoft) | Tasks.ReadWrite    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Prefira: outlook.timezone | Especifica o fuso horário para propriedades de tempo na resposta, que estaria em UTC se esse header não for especificado. Opcional.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir marca a tarefa especificada como concluída. Especifica o Horário Padrão do Pacífico (PST) no `Prefer: outlook.timezone` header.

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. As **propriedades completedDateTime** e outras relacionadas à data na resposta são expressas em PST.

> **Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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


