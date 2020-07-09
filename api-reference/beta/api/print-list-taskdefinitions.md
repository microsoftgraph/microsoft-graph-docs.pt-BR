---
title: Listar taskDefinitions
description: Recupere uma lista de definições de tarefas que o aplicativo solicitante definido no locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 91d00b7773b56d4c5f522981c7a59dde3744a710
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091555"
---
# <a name="list-taskdefinitions"></a>Listar taskDefinitions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [definições de tarefas](../resources/printtaskdefinition.md) que o aplicativo solicitante definido no locatário.

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
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).

### <a name="exceptions"></a>Exceptions
Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização | Bearer {token}. Required. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```

---

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
