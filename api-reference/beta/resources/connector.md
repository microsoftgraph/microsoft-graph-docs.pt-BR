---
title: tipo de recurso conector
description: Representa um conector de proxy de aplicativo.
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e42bc42c1989e530f7b7f307da3963407ded112
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027164"
---
# <a name="connector-resource-type"></a>tipo de recurso conector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os conectores são agentes leves que ficam no local e facilitam a conexão de saída para o serviço de [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) . Cada conector é parte de um [conector](connectorgroup.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/connector-list.md) | coleção [Connector](connector.md) | Recupere uma lista de objetos Connector. | 
| [Obter conector](../api/connector-get.md) | [conector](connector.md) | Leia as propriedades e as relações do objeto Connector. |
| [Listar memberOf](../api/connector-list-memberof.md) | coleção de [conectores](connectorgroup.md) | Lista o conjunto de objetos do grupo de conectores do qual o conector é membro. |
| [Adicionar conector a connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Adicionar um conector a um conector. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|String| O endereço IP externo, conforme detectado pelo servidor do conector. Somente leitura. |
|id|String| Identificador exclusivo do conector. Somente leitura. |
|Nomecomputador|String| O nome do computador no qual o conector está instalado e em execução. |
|status|cadeia de caracteres| Indica o status do conector. Os valores possíveis são: `active` e `inactive`. Somente leitura. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|memberOf|coleção de [conectores](connectorgroup.md)| O MemberGroup do qual o conector é membro. Somente leitura. |

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


