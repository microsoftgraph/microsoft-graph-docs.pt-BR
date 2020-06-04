---
title: tipo de recurso do The Connector
description: Representa uma conexão de proxy de aplicativo.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 446dae5e78878ba9648d532d2696b0bfde496601
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556167"
---
# <a name="connectorgroup-resource-type"></a>tipo de recurso do The Connector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cada conector de [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) é sempre parte de um grupo de conectores. Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para alta disponibilidade e balanceamento de carga. Se você não criar grupos de conectores, todos os seus conectores farão parte do grupo padrão. Ao configurar um aplicativo com o proxy de aplicativo, você também deve especificar o grupo de conectores ao qual o aplicativo será atribuído.

Depois que um grupo de conectores é criado, você pode adicionar ou mover conectores para o grupo de conectores usando [Adicionar conector](../api/connectorgroup-post-members.md). Você também pode usar [Adicionar aplicativo](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista de conectores de lista](../api/connectorgroup-list.md) |coleção de [conectores](connectorgroup.md) | Recupere uma lista de objetos de conexão. |
|[Obter um conector de conexão](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | Leia as propriedades e as relações de um objeto de conexão. |
|[Atualizar o beficador de conexão](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| Atualize um objeto de conexão. |
|[Excluir um ou de conector](../api/connectorgroup-delete.md) | Nenhuma | Excluir um objeto de um. Todos os conectores devem ser removidos do conector para que um dos conectores possa ser excluído. |
|[Listar membros](../api/connectorgroup-list-members.md) |coleção [Connector](connector.md)| Obtenha uma coleção de objetos Connector. |
|[Listar aplicativos](../api/connectorgroup-list-applications.md) |Coleção [application](application.md)| Obter a coleção de objetos Application associada ao grupo de conectores. |
|[Adicionar aplicativo](../api/connectorgroup-post-applications.md) |[aplicativo](application.md)| Associar um aplicativo ao grupo de conectores postando na coleção de aplicativos. |
|[Adicionar conector](../api/connectorgroup-post-members.md) |[conector](connector.md)| Adicionar um conector ao grupo de conectores postando na coleção de conectores. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|connectorGroupType|string| Indica o tipo de agente híbrido. Isso é definido pelo sistema. Somente leitura. |
|id|cadeia de caracteres| Identificador exclusivo desse conector. Somente leitura. |
|isDefault|booliano| Indica se o conector de conexão é o padrão. Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema. Somente leitura. |
|name|string| O nome associado ao conector. |
|região|string| A região à qual o conector é atribuído e otimizará o tráfego para o. Essa região só poderá ser definida se **nenhum conector ou aplicativo** for atribuído ao grupo de conectores. As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia. Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Emprego|Coleção [application](application.md)| Somente leitura. Anulável.|
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
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
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
