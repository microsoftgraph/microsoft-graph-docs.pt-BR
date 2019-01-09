---
title: 'outlookTask: completa'
description: 'Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** como a data atual, '
ms.openlocfilehash: 2a92fa0f95737581275f1b5516d68a7feab9578f
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771804"
---
# <a name="outlooktask-complete"></a>outlookTask: completa

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** como a data atual e a propriedade **status** para `completed`.

Se estiver Concluindo uma tarefa em uma série recorrente, na resposta, a coleção de tarefa conterá tarefa concluída na série e a próxima tarefa na série.

A propriedade **completedDateTime** representa a data quando a tarefa é concluída. Por padrão, a parte do tempo de **completedDateTime** é definida como meia-noite UTC.

Por padrão, esta operação (e as operações de tarefa POST, GET e PATCH) retorna propriedades relacionadas a data em UTC. Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Tasks.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Tasks.ReadWrite    |
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
| Prefira: outlook.timezone | Especifica o fuso horário para as propriedades de tempo na resposta, qual seria em UTC se este cabeçalho não for especificado. Opcional.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` código de resposta e o objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir marca a tarefa especificada como concluída. Hora oficial do Pacífico (PST) em Especifica o `Prefer: outlook.timezone` cabeçalho.

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. O **completedDateTime** e outras propriedades relacionadas a data na resposta são expressos em PST.

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->