---
title: tipo de recurso de programa
description: 'No recurso de revisões de acesso do Azure AD, um programa é um contêiner, mantendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para facilitar a localização de avaliações de acesso relacionadas.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f10ee2a54a310018d87500e5dd4f939d1fe38a0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443983"
---
# <a name="program-resource-type"></a>tipo de recurso de programa

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões de acesso do Azure AD, um programa é um contêiner, mantendo [controles](accessreviews-root.md) de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para facilitar a localização de avaliações de acesso relacionadas.  

Cada locatário que tenha avaliações de acesso do Azure AD no Azure tem um programa, `Default program` .  Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade. 


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programa](../api/program-create.md) |   [program](program.md)   |   Crie um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  [conjunto de](program.md) programas|   Obter uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      [Coleção programControl](programcontrol.md)| Obter uma coleção dos controles de um programa.|
|[Atualizar programa](../api/program-update.md) |   [program](program.md)|  Atualize um programa.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  O identificador atribuído ao recurso do programa.                    |
| `displayName`               |`String`                              |  O nome do programa.  Obrigatório durante a criação.                  |
| `description`               |`String`                              |  A descrição do programa.           |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | Controles associados ao programa. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


