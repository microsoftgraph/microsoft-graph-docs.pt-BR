---
title: Tipo de recurso qna
description: Representa uma pergunta e resposta (P&A) em Pesquisa da Microsoft.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b205c31b533affd63b9d38650e1dfe8aa1fb2e3d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337960"
---
# <a name="qna-resource-type"></a>Tipo de recurso qna

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

P&Assim como os resultados de resposta administrativa na página de resultados da pesquisa que fornecem respostas para palavras-chave de pesquisa específicas. P&Como permitir que os administradores respondam às perguntas do usuário diretamente na pesquisa em vez de fornecer um link para uma página da Web. Um Q&A tem muitas propriedades que permitem que os administradores façam recursos comuns mais acessíveis em sua organização.

Herda de [searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar qnas](../api/search-searchentity-list-qnas.md)|[coleção microsoft.graph.search.qna](../resources/search-qna.md)|Obter uma lista dos [objetos qna](../resources/search-qna.md) e suas propriedades.|
|[Criar qna](../api/search-searchentity-post-qnas.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Crie um novo [objeto qna](../resources/search-qna.md) .|
|[Obter qna](../api/search-qna-get.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Leia as propriedades e as relações de um [objeto qna](../resources/search-qna.md) .|
|[Atualizar qna](../api/search-qna-update.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Atualize as propriedades de um [objeto qna](../resources/search-qna.md) .|
|[Excluir qna](../api/search-qna-delete.md)|Nenhum(a)|Exclui um [objeto qna](../resources/search-qna.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo (GUID) para a qna. Herdado da [entidade](../resources/entity.md).|
|displayName|String|Pergunta exibida nos resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|descrição|String|Resposta exibida nos resultados da pesquisa. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Link de URL de Qna. Quando os usuários clicarem nesse qna nos resultados da pesquisa, eles irão para essa URL. Herdado [de searchAnswer](../resources/search-searchAnswer.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Detalhes do usuário que criou ou modificou a qna pela última vez. Herdado [de searchAnswer](../resources/search-searchAnswer.md). Somente leitura. |
|lastModifiedDateTime|DateTimeOffset| Timestamp de quando a qna é criada ou editada. Herdado [de searchAnswer](../resources/search-searchAnswer.md). Somente leitura.|
|availabilityStartDateTime|DateTimeOffset|Timestamp de quando a qna começará a aparecer como um resultado de pesquisa. Definir como `null` para sempre disponível.|
|availabilityEndDateTime|DateTimeOffset|Timestamp de quando a qna será parada para aparecer como um resultado de pesquisa. Definir como `null` para sempre disponível.|
|languageTags|Coleção de cadeias de caracteres|Uma lista de nomes de idiomas geograficamente específicos e em que essa QnA pode ser exibida. Cada valor de marca de idioma segue o padrão {language}-{REGION}. Como exemplo, é `en-US` inglês como usado nos Estados Unidos. Consulte [marcas de idioma com suporte](search-api-answers-overview.md#supported-language-tags) para a lista de valores possíveis. |
|plataformas|coleção microsoft.graph.devicePlatformType|Lista de dispositivos e sistemas operacionais capazes de exibir esse qna. Os valores possíveis são: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[coleção microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Variações de uma qna para diferentes países ou dispositivos. Use quando precisar mostrar conteúdo diferente para os usuários com base em seu dispositivo, país/região ou ambos. As configurações de data e grupo serão aplicadas a todas as variações.|
|palavras-chave|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Palavras-chave que disparam esse qna aparecem nos resultados da pesquisa.|
|state|microsoft.graph.search.answerState|Estado da qna. Os valores possíveis são: `published`, `draft`, `excluded`ou `unknownFutureValue`.|
|isSuggested|Booliano| True se essa qna foi sugerida ao administrador por um usuário ou foi minerada e sugerida pela Microsoft. Somente leitura.|
|groupIds|Coleção de cadeias de caracteres|Lista de grupos de segurança capazes de exibir esse qna.|


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

