---
title: tipo de recurso de acrônimo
description: Um acrônimo é uma resposta administrativa nos resultados da Pesquisa da Microsoft para definir acrônimos comuns em uma organização.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0201a3b76201825b13e069b52924eacca9077d9f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338134"
---
# <a name="acronym-resource-type"></a>tipo de recurso de acrônimo

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um acrônimo é uma resposta administrativa nos resultados da Pesquisa da Microsoft para definir acrônimos comuns em uma organização.

Herda de [searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar acrônimos](../api/search-searchentity-list-acronyms.md)|[coleção microsoft.graph.search.acronym](../resources/search-acronym.md)|Obter uma lista dos objetos [de acrônimo](../resources/search-acronym.md) e suas propriedades.|
|[Criar acrônimo](../api/search-searchentity-post-acronyms.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|Crie um novo [objeto de acrônimo](../resources/search-acronym.md) .|
|[Obter acrônimo](../api/search-acronym-get.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|Leia as propriedades e as relações de um [objeto de acrônimo](../resources/search-acronym.md) .|
|[Atualizar acrônimo](../api/search-acronym-update.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|Atualize as propriedades de um [objeto de acrônimo](../resources/search-acronym.md) .|
|[Excluir acrônimo](../api/search-acronym-delete.md)|Nenhum|Exclui um [objeto de acrônimo](../resources/search-acronym.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Uma breve descrição do acrônimo que fornece aos usuários mais informações sobre o acrônimo e o que ele representa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|displayName|Cadeia de caracteres|O formulário curto ou acrônimo real. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|id|String|O identificador exclusivo (GUID) do acrônimo. Herdado da [entidade](../resources/entity.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Detalhes do usuário que criou ou modificou o acrônimo pela última vez. Herdado [de searchAnswer](../resources/search-searchAnswer.md). Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Timestamp de quando o acrônimo é criado ou editado. Herdado [de searchAnswer](../resources/search-searchAnswer.md). Somente leitura.|
|standsFor|Coleção de cadeias de caracteres|O que o acrônimo significa.|
|state|microsoft.graph.search.answerState|Estado do acrônimo. Os valores possíveis são: `published`, `draft`, `excluded`ou `unknownFutureValue`.|
|webUrl|String|A URL da página ou site onde os usuários podem ir para obter mais informações sobre o acrônimo. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.acronym",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.acronym",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "standsFor": [
    "String"
  ],
  "state": "String"
}
```

