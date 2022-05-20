---
title: tipo de recurso qna
description: Representa uma pergunta e resposta (Q&A) em Pesquisa da Microsoft.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d17f10b3613bb4e88791c90fd81e0440ece8eb2d
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602781"
---
# <a name="qna-resource-type"></a>tipo de recurso qna

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

P&Assim como os resultados da resposta administrativa na página de resultados da pesquisa que fornecem respostas para palavras-chave de pesquisa específicas. P&Como permitir que os administradores respondam às perguntas do usuário diretamente na pesquisa em vez de fornecer um link para uma página da Web. Um Q&A tem muitas propriedades que permitem aos administradores tornar os recursos comuns mais acessíveis em sua organização.

Herda de [searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar qnas](../api/search-searchentity-list-qnas.md)|[coleção microsoft.graph.search.qna](../resources/search-qna.md)|Obtenha uma lista dos [objetos qna](../resources/search-qna.md) e suas propriedades.|
|[Criar qna](../api/search-searchentity-post-qnas.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Crie um novo [objeto qna](../resources/search-qna.md) .|
|[Obter qna](../api/search-qna-get.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Leia as propriedades e as relações de um [objeto qna](../resources/search-qna.md) .|
|[Atualizar qna](../api/search-qna-update.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Atualize as propriedades de um [objeto qna](../resources/search-qna.md) .|
|[Excluir qna](../api/search-qna-delete.md)|Nenhum|Exclui um [objeto qna](../resources/search-qna.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID (identificador exclusivo) para o qna. Herdado da [entidade](../resources/entity.md).|
|displayName|Cadeia de caracteres|Pergunta exibida nos resultados da pesquisa. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|descrição|Cadeia de caracteres|Resposta exibida nos resultados da pesquisa. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link da URL do Qna. Quando os usuários clicarem nesse qna nos resultados da pesquisa, eles acessarão essa URL. Herdado de [searchAnswer](../resources/search-searchAnswer.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Detalhes do usuário que criou ou modificou o qna pela última vez. Herdado de [searchAnswer](../resources/search-searchAnswer.md). Somente leitura. |
|lastModifiedDateTime|DateTimeOffset| Carimbo de data/hora de quando o qna é criado ou editado. Herdado de [searchAnswer](../resources/search-searchAnswer.md). Somente leitura.|
|availabilityStartDateTime|DateTimeOffset|Carimbo de data/hora de quando o qna começará a aparecer como um resultado de pesquisa. Defina `null` como sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Carimbo de data/hora de quando o qna será interrompido para aparecer como um resultado de pesquisa. Defina `null` como sempre disponível.|
|languageTags|Coleção de cadeias de caracteres|Uma lista de nomes de idioma que são geograficamente específicos e que esse QnA pode ser exibido. Cada valor de marca de idioma segue o padrão {language}-{region}. Por exemplo, é `en-us` inglês conforme usado no Estados Unidos. Consulte [as marcas de idioma com suporte](search-api-answers-overview.md#supported-language-tags) para obter a lista de valores possíveis. |
|Plataformas|Coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse qna. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de um qna para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse qna para aparecer nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado do qna. Os valores possíveis são`draft`: `published`, , `excluded`ou `unknownFutureValue`.|
|isSuggested|Booleano| True se essa qna foi sugerida ao administrador por um usuário ou foi minerada e sugerida pela Microsoft. Somente leitura.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir este qna.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.qna",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.qna",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
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

