---
title: Atualizar outlooktask
description: Alterar propriedades writable de uma Outlook tarefa.
author: mashriv
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 44f74ee7c9c46a352c49f9ca79cbe1684013ed41
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011567"
---
# <a name="update-outlooktask-deprecated"></a>Atualizar outlooktask (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Alterar propriedades writable de uma Outlook tarefa.

A **propriedade completedDateTime** pode ser definida pela **ação completa** ou explicitamente por uma operação PATCH. Se você usar PATCH para definir **completedDateTime**, certifique-se de definir **o status** `completed` como também.

Por padrão, essa operação (e as [](../api/outlooktask-complete.md) operações DE TAREFA POST, GET e concluída) retorna propriedades relacionadas à data em UTC. Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.

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
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | {token} de portador. Obrigatório. |
| Prefira: outlook.timezone | Especifica o fuso horário para propriedades de tempo na resposta, que estaria em UTC se esse header não for especificado. Opcional.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|corpo|[itemBody](../resources/itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa. Observe para qual tipo de HTML há suporte.|
|Categorias|Coleção de cadeias de caracteres|As categorias associadas à postagem.|
|changeKey|Cadeia de caracteres|A versão da tarefa.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa foi concluída.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída.|
|hasAttachments|Booliano|Defina como verdadeiro se a tarefa tiver anexos.|
|importância|cadeia de caracteres|A importância do evento. Os valores possíveis são: `low`, `normal` e `high`.|
|isReminderOn|Booliano|Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|owner|Cadeia de caracteres|O nome da pessoa que criou a tarefa.|
|parentFolderId|Cadeia de caracteres|O identificador exclusivo para a pasta pai da tarefa.|
|recorrência|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data e hora do alerta de lembrete da tarefa.|
|sensibilidade|cadeia de caracteres|Indica o nível de privacidade da tarefa. Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será iniciada.|
|status|cadeia de caracteres|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|assunto|Cadeia de caracteres|Uma breve descrição ou o título da tarefa.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [outlookTask](../resources/outlooktask.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

O exemplo a seguir modifica a **propriedade dueDateTime** e usa o header para especificar a expressão das propriedades relacionadas à data na resposta em Horário Padrão do Leste `Prefer: outlook.timezone` (EST).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTHgwAAA=
Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-outlooktask-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
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
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
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
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


