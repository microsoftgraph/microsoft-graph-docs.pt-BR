---
title: Tipo de recurso connectorGroup
description: Representa um Application Proxy connectorGroup.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: df3a80c6dfd4004daccfe33045c8775c2e2e6e48
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958805"
---
# <a name="connectorgroup-resource-type"></a>Tipo de recurso connectorGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cada conector proxy de aplicativo [do Azure AD](https://aka.ms/whyappproxy) sempre faz parte de um grupo de conectores. Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para balanceamento de carga e alta disponibilidade. Se você não criar grupos de conectores, todos os conectores serão parte do grupo padrão. Ao configurar um aplicativo com Proxy de Aplicativo, você também deve especificar a qual grupo de conectores atribuir o aplicativo.

Depois que um grupo de conectores for criado, você poderá adicionar ou mover conectores para o grupo do conector usando [Add connector](../api/connectorgroup-post-members.md). Você também pode usar [o aplicativo Add](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar connectorGroup](../api/connectorgroup-list.md) |[Coleção connectorGroup](connectorgroup.md) | Recupere uma lista de objetos connectorGroup. |
|[Criar connectorGroup](../api/connectorgroup-post.md) |[Coleção connectorGroup](connectorgroup.md) | Crie um objeto connectorGroup. |
|[Obter connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | Ler propriedades e relações de um objeto connectorGroup. |
|[Atualizar connectorGroup](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| Atualize um objeto connectorGroup. |
|[Excluir connectorGroup](../api/connectorgroup-delete.md) | Nenhum | Exclua um objeto connectorGroup. Todos os conectores devem ser removidos do connectorGroup antes que um connectorGroup possa ser excluído. |
|[Listar membros](../api/connectorgroup-list-members.md) |[coleção connector](connector.md)| Obter uma coleção de objetos do conector. |
|[Listar aplicativos](../api/connectorgroup-list-applications.md) |Coleção [application](application.md)| Obter a coleção de objetos de aplicativo associada ao connectorGroup. |
|[Adicionar aplicativo](../api/connectorgroup-post-applications.md) |[application](application.md)| Associe um aplicativo ao connectorGroup postando na coleção applications. |
|[Adicionar conector](../api/connectorgroup-post-members.md) |[connector](connector.md)| Adicione um conector ao connectorGroup postando na coleção connectorGroup. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|connectorGroupType|connectorGroupType| Indica o tipo de agente híbrido. Este pré-definido pelo sistema. Os valores possíveis são: `applicationProxy` . Somente leitura. |
|id|cadeia de caracteres| Identificador exclusivo para este connectorGroup. Somente leitura. |
|isDefault|booliano| Indica se o connectorGroup é o connectorGroup padrão. Somente um único grupo de conectores pode ser o connectorGroup padrão e isso é pré-definido pelo sistema. Somente leitura. |
|name|string| O nome associado ao connectorGroup. |
|region|connectorGroupRegion| A região à que o connectorGroup é atribuído e otimizará o tráfego. Essa região só poderá ser definida se **nenhum conector ou aplicativo** for atribuído ao connectorGroup. Os valores possíveis são: `nam` (para **a América do Norte**), (para a `eur` Europa), (para a `aus` Austrália), (para a `asia` Ásia), `ind` (para a Índia) e `unknownFutureValue` .|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|applications|Coleção [application](application.md)| Somente leitura. Anulável.|
|members|[coleção connector](connector.md)| Somente leitura. Anulável.|

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



