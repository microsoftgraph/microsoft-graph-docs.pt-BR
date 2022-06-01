---
title: tipo de recurso de programa (preterido)
description: 'No recurso Azure AD revisões de acesso, um programa é um contêiner, mantendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa para facilitar a localização de revisões de acesso relacionadas.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f0d0a7a42a21a95bbf57b971d09e20046bd46ffa
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819395"
---
# <a name="program-resource-type-deprecated"></a>tipo de recurso de programa (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões de acesso](accessreviews-root.md), um programa é um contêiner, mantendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa para facilitar a localização de revisões de acesso relacionadas.  

Cada locatário que tem revisões de acesso Azure AD internas tem um programa, `Default program`.  Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programa](../api/program-create.md) |   [Programa](program.md)   |   Crie um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  [coleção de](program.md) programas|   Obtenha uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      [coleção programControl](programcontrol.md)| Obtenha uma coleção dos controles de um programa.|
|[Atualizar programa](../api/program-update.md) |   [Programa](program.md)|  Atualizar um programa.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id                        |Cadeia de caracteres                              |  O identificador atribuído ao recurso do programa.                    |
| displayName               |String                              |  O nome do programa.  Obrigatório durante a criação.                  |
| description               |Cadeia de caracteres                              |  A descrição do programa.           |

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


