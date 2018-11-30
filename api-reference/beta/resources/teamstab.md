---
title: tipo de recurso de teamsTab
description: 'Um teamsTab é uma guia que tem fixados (anexado) a um canal de uma equipe. '
ms.openlocfilehash: cba82432f6ade7baa591c3abb7e099ec7f6e9d5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036637"
---
# <a name="teamstab-resource-type"></a>tipo de recurso de teamsTab

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um teamsTab é uma [guia](../resources/teamstab.md) que tem fixados (anexado) a um [canal](channel.md) de dentro de uma [equipe](team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Guias de lista](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Guias de listas fixados em um canal.|
|[Obtenha o guia](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Lê uma guia fixada em um canal.|
|[Adicionar guia](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Adiciona (pins) uma guia em um canal.|
|[Remover guia](../api/teamstab-delete.md) | Nenhum | Remove (unpin) uma guia de um canal.|
|[Guia de atualização](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Atualiza as propriedades da guia.|


## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|  id              |   string                  |  Identificador que identifica exclusivamente uma instância específica de um canal na guia leitura apenas.     |
|  displayName            |   string                  |  Nome da guia.     |
|  name            |   string                  |  (Obsoleto) Nome da guia.     |
|  teamsAppId           |   string             |  Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação da guia.     |
|  sortOrderIndex  |   inteiro                     |  Índice da ordem usada para classificar as guias     |
|  webUrl          |   string                  |  Link profundo url da instância do guia. Somente leitura.     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Contêiner de configurações personalizadas aplicadas a uma guia. Na guia é considerada configurado somente depois que essa propriedade for definida.     |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | O aplicativo que está vinculado à guia. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Confira também

[Configurando os tipos de guia interna](/graph/teams-configuring-builtin-tabs)
