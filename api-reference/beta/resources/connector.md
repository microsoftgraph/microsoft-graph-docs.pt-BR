---
title: tipo de recurso conector
description: Representa um conector de proxy de aplicativo.
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864d76d7e6a7cb3724a91a753e5c5198e274780a
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556174"
---
# <a name="connector-resource-type"></a>tipo de recurso conector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os conectores são agentes leves que ficam no local e facilitam a conexão de saída para o serviço de [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) . Cada conector é parte de um [conector](connectorgroup.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Conectores de lista](../api/connector-list.md) | coleção [Connector](connector.md) | Recupere uma lista de objetos Connector. | 
| [Obter conector](../api/connector-get.md) | [conector](connector.md) | Leia as propriedades e as relações do objeto Connector. |
| [Listar memberOf](../api/connector-list-memberof.md) | coleção de [conectores](connectorgroup.md) | Lista o conjunto de objetos do grupo de conectores do qual o conector é membro. |
| [Adicionar conector ao conector](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Adicionar um conector a um conector. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|String| O endereço IP externo, conforme detectado pelo servidor do conector. Somente leitura. |
|id|Cadeia de caracteres| Identificador exclusivo do conector. Somente leitura. |
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
