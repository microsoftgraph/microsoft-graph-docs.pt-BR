---
title: tipo de recurso de indicador
description: Um indicador é uma resposta administrativa em Pesquisa da Microsoft resultados para consultas comuns de pesquisa em uma organização. Um indicador tem muitas propriedades que permitem aos administradores tornar os recursos comuns mais acessíveis em sua organização.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 24582a18ae2ad332a59bc3d8b2db28b3e3189b6a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337961"
---
# <a name="bookmark-resource-type"></a>tipo de recurso de indicador

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um indicador é uma resposta administrativa em Pesquisa da Microsoft resultados para consultas comuns de pesquisa em uma organização. Um indicador tem muitas propriedades que permitem aos administradores tornar os recursos comuns mais acessíveis em sua organização.

Herda de [searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar indicadores](../api/search-searchentity-list-bookmarks.md)|[coleção microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Obter uma lista dos objetos [de indicador](../resources/search-bookmark.md) e suas propriedades.|
|[Criar indicador](../api/search-searchentity-post-bookmarks.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Crie um novo [objeto bookmark](../resources/search-bookmark.md) .|
|[Obter indicador](../api/search-bookmark-get.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Leia as propriedades e as relações de um [objeto bookmark](../resources/search-bookmark.md) .|
|[Atualizar indicador](../api/search-bookmark-update.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Atualize as propriedades de [um objeto bookmark](../resources/search-bookmark.md) .|
|[Excluir indicador](../api/search-bookmark-delete.md)|Nenhum(a)|Exclui um [objeto bookmark](../resources/search-bookmark.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo (GUID) do indicador. Herdado da [entidade](../resources/entity.md).|
|displayName|String|Nome do indicador exibido nos resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|descrição|String|Descrição do indicador mostrada na página de resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link da URL do indicador. Quando os usuários clicarem nesse indicador nos resultados da pesquisa, eles irão para essa URL. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Detalhes do usuário que criou ou modificou o indicador pela última vez. Herdado [de searchAnswer](../resources/search-searchAnswer.md). Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador é criado ou editado. Herdado [de searchAnswer](../resources/search-searchAnswer.md). Somente leitura. |
|categories|String collection|Categorias comumente usadas para descrever esse indicador. Por exemplo, IT e RH.|
|availabilityStartDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador começará a aparecer como um resultado de pesquisa. Definir como `null` para sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Carimbo de data/hora de quando o indicador será parar para aparecer como resultado da pesquisa. Definir como `null` para sempre disponível.|
|languageTags|String collection|Uma lista de nomes de idiomas geograficamente específicos e em que esse indicador pode ser exibido. Cada valor de marca de idioma segue o padrão {language}-{REGION}. Como exemplo, é `en-US` inglês como usado nos Estados Unidos. Consulte [marcas de idioma com suporte](search-api-answers-overview.md#supported-language-tags) para a lista de valores possíveis.|
|plataformas|coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse indicador. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de um indicador para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|powerAppIds|Coleção de cadeias de caracteres|Lista de Power Apps associados a esse indicador. Se os usuários adicionarem Power Apps existentes a um indicador, eles poderão concluir tarefas, como inserir o período de férias ou relatar despesas na página de resultados da pesquisa.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse indicador aparecem nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado do indicador. Os valores possíveis são: `published`, `draft`, `excluded`ou `unknownFutureValue`.|
|isSuggested|Booliano|True se esse indicador foi sugerido ao administrador por um usuário ou foi minerado e sugerido pela Microsoft. Somente leitura.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir esse indicador.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.bookmark",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.bookmark",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "categories": [
    "String"
  ],
  "availabilityStartDateTime": "String (timestamp)",
  "availabilityEndDateTime": "String (timestamp)",
  "languageTags": [
    "String"
  ],
  "platforms": [
    "String"
  ],
  "targetedVariations": [
    {
      "@odata.type": "microsoft.graph.search.answerVariant"
    }
  ],
  "powerAppIds": [
    "String"
  ],
  "keywords": {
    "@odata.type": "microsoft.graph.search.answerKeyword"
  },
  "state": "String",
  "isSuggested": "Boolean",
  "groupIds": [
    "String"
  ]
}
```

