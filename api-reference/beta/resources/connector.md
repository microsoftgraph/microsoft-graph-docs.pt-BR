---
title: tipo de recurso conector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25d350e48aaddbda2b931ae5a9e177ec6caa9799
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507475"
---
# <a name="connector-resource-type"></a>tipo de recurso conector

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter conector](../api/connector-get.md) | [conector](connector.md) |Leia as propriedades e as relações do objeto Connector.|
|[Listar memberOf](../api/connector-list-memberof.md) |coleção de [conectores](connectorgroup.md)| Obtenha o objeto de conexão associado ao conector.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|externalIp|String|O endereço IP externo, conforme detectado pelo serviço para o computador do conector. Somente leitura|
|id|Cadeia de caracteres| A ID de objeto do conector. <BR>Somente leitura.|
|Nomecomputador|String| O nome da máquina na qual o conector está sendo executado. <BR>Somente leitura|
|status|cadeia de caracteres| Indica o status do conector. Os valores possíveis são: `active` e `inactive`. Somente leitura |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|memberOf|coleção de [conectores](connectorgroup.md)| O MemberGroup do qual a conexão é membro.<br>Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
