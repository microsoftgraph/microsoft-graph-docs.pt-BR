---
title: Criar taskTrigger
description: Criar um novo disparador de tarefas na impressora especificada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 453759faf24ac5c116e3f1d9bf73aa7771aae595
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091591"
---
# <a name="create-tasktrigger"></a>Criar taskTrigger

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo [disparador de tarefas](../resources/printtasktrigger.md) na [impressora](../resources/printer.md)especificada. No momento, apenas **um** gatilho de tarefa pode ser especificado por impressora, mas esse limite pode ser removido no futuro. Além disso, somente o aplicativo que registrou a impressora pode gerenciar seus gatilhos de tarefa.

## <a name="permissions"></a>Permissões
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Printer. ReadWrite. All, Printer. FullControl. All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização | Bearer {token}. Required. |
| Content-type  | application/json. Required.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [printTaskTrigger](../resources/printtasktrigger.md) . Forneça uma referência a um [printTaskDefinition](../resources/printtaskdefinition.md) usando o `@odata.bind` formato, conforme mostrado no exemplo a seguir.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_printer_tasktrigger"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
}
```

---

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 196

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```
