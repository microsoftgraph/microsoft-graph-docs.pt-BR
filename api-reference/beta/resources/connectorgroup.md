---
title: tipo de recurso de connectorGroup
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: a3131b887216f1f400f70ed8d607477f65793cc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038205"
---
# <a name="connectorgroup-resource-type"></a>tipo de recurso de connectorGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Leia as propriedades e os relacionamentos do objeto connectorGroup.|
|[Criar aplicativo](../api/connectorgroup-post-applications.md) |[application](application.md)| Associe um aplicativo com o grupo de conector pelo lançamento para o conjunto de aplicativos.|
|[Lista de aplicativos](../api/connectorgroup-list-applications.md) |conjunto de [aplicativos](application.md)| Obter a coleção de objeto do aplicativo associado.|
|[Criar um conector](../api/connectorgroup-post-members.md) |[conector](connector.md)| Adicione um conector para o grupo de conector pelo lançamento para o conjunto de membros.|
|[Listar membros](../api/connectorgroup-list-members.md) |coleção de [conector](connector.md)| Obtenha um conector a coleção de objetos.|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |Atualize o objeto connectorGroup. |
|[Delete](../api/connectorgroup-delete.md) | Nenhum |Exclua objeto connectorGroup. Todos os conectores devem ser remove antes de um conector de grupo pode ser excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|connectorGroupType|string| O tipo de conectores que será usado com o grupo. Os valores possíveis são: `applicationProxy`.|
|id|String| O id de objeto do connectorGroup|
|isDefault|Booliano| Indica se o connectorGroup é o grupo de conector padrão. Apenas um conector grupo pode ser o connectorGroup padrão e é definido pelo sistema.|
|name|String| O nome associado a connectorGroup.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|aplicativos|conjunto de [aplicativos](application.md)| Somente leitura. Anulável.|
|membros|coleção de [conector](connector.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
