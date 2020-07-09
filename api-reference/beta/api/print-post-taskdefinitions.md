---
title: Criar taskDefinition
description: Criar uma nova definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 147e1271ee0f5bcd7c04e167e172c48939a4da98
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091552"
---
# <a name="create-taskdefinition"></a>Criar taskDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar uma nova definição de tarefa.

Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="permissions"></a>Permissões
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Sem suporte. |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| PrintTaskDefinition. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização | Bearer {token}. Required. |
| Content-type  | application/json. Required.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [printTaskDefinition](../resources/printtaskdefinition.md) .

As propriedades **ID** e **createdBy. AppID** do [printTaskDefinition](../resources/printtaskdefinition.md)são definidas automaticamente na criação de recurso.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "print_create_taskdefinition"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/print/taskDefinitions
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

---

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 322

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
