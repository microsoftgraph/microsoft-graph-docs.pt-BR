---
title: tipo de recurso do conector
description: Representa um conector proxy de aplicativo.
author: japere
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d88d7468872fb4e0e6b8d6ae5dd84346ba7de36a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136684"
---
# <a name="connector-resource-type"></a>tipo de recurso do conector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os conectores são agentes leves que se sentam no local e facilitam a conexão de saída para o serviço proxy de aplicativo do [Azure AD.](/azure/active-directory/app-proxy/what-is-application-proxy) Cada conector faz parte de um [connectorGroup](connectorgroup.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/connector-list.md) | [coleção connector](connector.md) | Recupere uma lista de objetos do conector. | 
| [Obter conector](../api/connector-get.md) | [connector](connector.md) | Ler propriedades e relações do objeto connector. |
| [Listar memberOf](../api/connector-list-memberof.md) | [Coleção connectorGroup](connectorgroup.md) | Listar a coleção de objetos connectorGroup da que o conector é membro. |
| [Adicionar conector a connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Adicione um conector a um connectorGroup. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|Cadeia de caracteres| O endereço IP externo detectado pelo servidor do conector. Somente leitura. |
|id|Cadeia de caracteres| Identificador exclusivo do conector. Somente leitura. |
|machineName|Cadeia de caracteres| O nome do computador em que o conector está instalado e em execução. |
|status|connectorStatus| Indica o status do conector. Os valores possíveis são: `active` e `inactive`. Somente leitura. |

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