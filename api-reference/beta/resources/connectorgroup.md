---
title: Tipo de recurso connectorGroup
description: Representa um Application Proxy connectorGroup.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 78716646f4bf5cbba7a66da4cdef88d94d1984aa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132318"
---
# <a name="connectorgroup-resource-type"></a>Tipo de recurso connectorGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cada [conector de Proxy de Aplicativo do Azure AD](https://aka.ms/whyappproxy) sempre faz parte de um grupo de conectores. Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para alta disponibilidade e balanceamento de carga. Se você não criar grupos de conectores, todos os conectores serão parte do grupo padrão. Ao configurar um aplicativo com o Proxy de Aplicativo, você também deve especificar a qual grupo de conector atribuir o aplicativo.

Depois que um grupo de conectores é criado, você pode adicionar ou mover conectores para o grupo de conectores usando [Adicionar conector.](../api/connectorgroup-post-members.md) Você também pode usar [Adicionar aplicativo](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar connectorGroup](../api/connectorgroup-list.md) |[Coleção connectorGroup](connectorgroup.md) | Recupere uma lista de objetos connectorGroup. |
|[Criar connectorGroup](../api/connectorgroup-post.md) |[Coleção connectorGroup](connectorgroup.md) | Crie um objeto connectorGroup. |
|[Obter connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | Ler propriedades e relações de um objeto connectorGroup. |
|[Atualizar connectorGroup](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| Atualize um objeto connectorGroup. |
|[Excluir connectorGroup](../api/connectorgroup-delete.md) | Nenhuma | Exclua um objeto connectorGroup. Todos os conectores devem ser removidos do connectorGroup antes que um connectorGroup possa ser excluído. |
|[Listar membros](../api/connectorgroup-list-members.md) |[conjunto de conectores](connector.md)| Obter uma coleção de objetos do conector. |
|[Listar aplicativos](../api/connectorgroup-list-applications.md) |Coleção [application](application.md)| Obter a coleção de objetos de aplicativo associada ao connectorGroup. |
|[Adicionar aplicativo](../api/connectorgroup-post-applications.md) |[aplicativo](application.md)| Associe um aplicativo ao connectorGroup postando na coleção applications. |
|[Adicionar conector](../api/connectorgroup-post-members.md) |[connector](connector.md)| Adicione um conector ao connectorGroup postando na coleção connectorGroup. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|connectorGroupType|string| Indica o tipo de agente híbrido. Isso é pré-definido pelo sistema. Somente leitura. |
|id|string| Identificador exclusivo deste connectorGroup. Somente leitura. |
|isDefault|booliano| Indica se o connectorGroup é o connectorGroup padrão. Somente um único grupo de conectores pode ser o connectorGroup padrão e isso é pré-definido pelo sistema. Somente leitura. |
|name|string| O nome associado ao connectorGroup. |
|region|string| A região à que o connectorGroup está atribuído e otimizará o tráfego. Essa região só poderá ser definida se **nenhum conector ou aplicativo** estiver atribuído ao connectorGroup. As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia. Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|applications|Coleção [application](application.md)| Somente leitura. Anulável.|
|members|[conjunto de conectores](connector.md)| Somente leitura. Anulável.|

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



