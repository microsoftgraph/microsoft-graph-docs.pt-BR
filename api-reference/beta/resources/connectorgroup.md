---
title: tipo de recurso do The Connector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d985f1f49ade4057b1a9ed9d3e1dbdafebfec7f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973189"
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
|[Atualização](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |Atualize o objeto de conexão. |
|[Delete](../api/connectorgroup-delete.md) | Nenhum |Exclua objeto de conexão. Todos os conectores devem ser removidos para que um grupo do conector possa ser excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|connectorGroupType|string| O tipo de conectores que serão usados com o grupo. Os valores possíveis são `applicationProxy`:.|
|id|String| A ID do objeto do conector|
|isDefault|Booliano| Indica se o grupo de conectores é o padrão. Somente um grupo de conectores único pode ser o grupo de conectores padrão e é definido pelo sistema.|
|name|String| O nome associado ao conector.|

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
