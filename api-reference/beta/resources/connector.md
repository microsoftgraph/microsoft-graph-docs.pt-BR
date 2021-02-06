---
title: tipo de recurso do conector
description: Representa um conector de Proxy de Aplicativo.
author: japere
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 53a5726456ce3d03ea537e87ec0dddb901623601
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136767"
---
# <a name="connector-resource-type"></a>tipo de recurso do conector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Conectores são agentes leves que ficam no local e facilitam a conexão de saída com o serviço de Proxy de Aplicativo do [Azure AD.](https://aka.ms/whyappproxy) Cada conector faz parte de um [connectorGroup](connectorgroup.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/connector-list.md) | [conjunto de conectores](connector.md) | Recupere uma lista de objetos de conector. | 
| [Obter conector](../api/connector-get.md) | [connector](connector.md) | Leia as propriedades e os relacionamentos do objeto connector. |
| [Listar memberOf](../api/connector-list-memberof.md) | [Coleção connectorGroup](connectorgroup.md) | Listar a coleção de objetos connectorGroup da que o conector é membro. |
| [Adicionar conector a connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Adicione um conector a um connectorGroup. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|String| O endereço IP externo detectado pelo servidor do conector. Somente leitura. |
|id|String| Identificador exclusivo do conector. Somente leitura. |
|machineName|String| O nome do computador em que o conector está instalado e em execução. |
|status|cadeia de caracteres| Indica o status do conector. Os valores possíveis são: `active` e `inactive`. Somente leitura. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|memberOf|[Coleção connectorGroup](connectorgroup.md)| O connectorGroup do que o conector é membro. Somente leitura. |

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



