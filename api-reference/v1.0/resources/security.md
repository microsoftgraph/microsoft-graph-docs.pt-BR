---
title: tipo de recurso de segurança
description: O recurso de segurança é o ponto de entrada para o modelo de objeto de segurança. Ele retorna um recurso de segurança singleton. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 87bd321a3c5e66cdc5d4fdc7fcb1407d02fbca1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034451"
---
# <a name="security-resource-type"></a>tipo de recurso de segurança

O recurso de segurança é o ponto de entrada para o modelo de objeto de segurança. Ele retorna um recurso de segurança singleton. Ele não contém propriedades utilizáveis.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar alertas](../api/alert-list.md) | conjunto [alerta](alert.md)  | Obtenha uma coleção de objetos de alerta. |
| [obter alertas](../api/alert-get.md) | conjunto [alerta](alert.md)  | Obter um objeto de alerta. |
| [Atualizar alertas](../api/alert-update.md) | conjunto [alerta](alert.md)  | Obter um objeto de alerta. |

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|alerts|conjunto [alerta](alert.md) | Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>Exemplo

O recurso de **segurança** está disponível na raiz do gráfico.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
