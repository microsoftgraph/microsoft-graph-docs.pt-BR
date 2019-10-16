---
title: tipo de recurso do The Connector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 02ef418f0f2124b4bd0c7489db8c732398005761
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538382"
---
# <a name="connectorgroup-resource-type"></a>tipo de recurso do The Connector

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter um conector de conexão](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Leia as propriedades e as relações do objeto de conexão.|
|[Criar aplicativo](../api/connectorgroup-post-applications.md) |[application](application.md)| Associe um aplicativo ao grupo de conectores postando na coleção de aplicativos.|
|[Listar aplicativos](../api/connectorgroup-list-applications.md) |coleção [Application](application.md)| Obtenha a coleção de objetos de aplicativo associada.|
|[Criar conector](../api/connectorgroup-post-members.md) |[conector](connector.md)| Adicionar um conector ao grupo de conectores postando na coleção Members.|
|[Listar membros](../api/connectorgroup-list-members.md) |coleção [Connector](connector.md)| Obtenha uma coleção de objetos Connector.|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |Atualize o objeto de conexão. |
|[Delete](../api/connectorgroup-delete.md) | Nenhum |Exclua objeto de conexão. Todos os conectores devem ser removidos para que um grupo de conectores possa ser excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|connectorGroupType|string| O tipo de conectores que serão usados com o grupo. Os valores possíveis são `applicationProxy`:.|
|id|String| A ID do objeto do conector|
|isDefault|Booliano| Indica se o grupo de conectores é o padrão. Somente um grupo de conectores único pode ser o grupo de conectores padrão e é definido pelo sistema.|
|name|Cadeia de caracteres| O nome associado ao conector.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Emprego|coleção [Application](application.md)| Somente leitura. Anulável.|
|members|coleção [Connector](connector.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
