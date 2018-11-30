---
title: tipo de recurso de conector
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039596"
---
# <a name="connector-resource-type"></a>tipo de recurso de conector

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obtenha o conector](../api/connector-get.md) | [conector](connector.md) |Leia as propriedades e os relacionamentos de objeto de conector.|
|[Listar memberOf](../api/connector-list-memberof.md) |coleção [connectorGroup](connectorgroup.md)| Obtenha o objeto de connectorGroup associado com o conector.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|externalIp|String|O endereço IP externo como detectada pelo serviço para a máquina do conector. Somente leitura|
|id|String| A id de objeto do conector. <BR>Somente leitura.|
|machineName|String| O nome do computador que está executando o conector. <BR>Somente leitura|
|status|string| Indica o status do conector. Os valores possíveis são: `active` e `inactive`. Somente leitura |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|memberOf|coleção [connectorGroup](connectorgroup.md)| O connectorGroup conectar é membro de.<br>Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
