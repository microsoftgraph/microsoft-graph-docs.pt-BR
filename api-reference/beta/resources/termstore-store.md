---
title: tipo de recurso Store
description: Representa um repositório de termos de taxonomia.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de8b0c004da804a4d9a617eec20de22c51e98108
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258421"
---
# <a name="store-resource-type"></a>tipo de recurso Store

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um repositório de termos de taxonomia.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição
|:---|:---|:---
|[Listar grupos](../api/termstore-list-groups.md)|coleção [Microsoft. Graph. termos. Group](../resources/termstore-group.md)| Obtenha os grupos de disponíveis no objeto do repositório de termos.|
|[Obter repositório](../api/termstore-store-get.md) | [Microsoft. Graph. termos. Store](../resources/termstore-store.md) | Leia as propriedades e os relacionamentos de um objeto do repositório de termos.
|[Atualizar repositório](../api/termstore-store-update.md) | [Microsoft. Graph. termos. Store](../resources/termstore-store.md) | Atualizar as propriedades de um objeto do repositório de termos.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição
|:---|:---|:---
|defaultLanguageTag | String | Idioma padrão do repositório de termos.
|id|String | Identificador exclusivo do repositório de termos. Somente leitura.
|languageTags | Coleção String | Lista de idiomas para o repositório de termos.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição
|:---|:---|:---
|grupos |coleção [Microsoft. Graph. termos. Group](../resources/termstore-group.md) | Coleção de todos os grupos disponíveis no repositório de termos.
|jogos | coleção [Microsoft. Graph. termos. Set](../resources/termstore-set.md) | Coleção de todos os conjuntos disponíveis no repositório de termos.


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->



