---
title: tipo de recurso de programa
description: 'No recurso de revisões do Azure AD Access, um programa é um contêiner, contendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a44c084b6f6d2da23290d3e962e2868f0c4c7ac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521450"
---
# <a name="program-resource-type"></a>tipo de recurso de programa

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](accessreviews-root.md) , um programa é um contêiner, contendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.  

Cada locatário que tem revisões de acesso do Azure AD integradas tem um programa, `Default program`.  Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programa](../api/program-create.md) |   [programa](program.md)   |   Criar um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  coleção [Program](program.md)|   Obtenha uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção de controles de um programa.|
|[Programa de atualização](../api/program-update.md) |   [programa](program.md)|  Atualizar um programa.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  O identificador do programa atribuído ao recurso.                    |
| `displayName`               |`String`                              |  O nome do programa.  Obrigatório ao criar.                  |
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
