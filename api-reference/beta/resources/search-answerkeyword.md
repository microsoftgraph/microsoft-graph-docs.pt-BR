---
title: Tipo de recurso answerKeyword
description: Palavras-chave de resposta permitem que os usuários definam palavras e frases que dispararão uma resposta de pesquisa administrativa para aparecer nos resultados da pesquisa.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b63a3a286528c7b1e7a1f87759cf7635499bde01
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338119"
---
# <a name="answerkeyword-resource-type"></a>Tipo de recurso answerKeyword

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma palavra-chave de resposta é usada para configurar palavras e frases que dispararão uma resposta de pesquisa administrativa para aparecer nos resultados da pesquisa.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|palavras-chave|Coleção de cadeias de caracteres|Uma coleção de palavras-chave usadas para disparar a resposta de pesquisa.|
|matchSimilarKeywords|Booliano|If `true`, indica que o termo de pesquisa contém palavras semelhantes às palavras-chave que devem disparar a resposta de pesquisa.|
|reservedKeywords|Coleção de cadeias de caracteres|Palavras-chave exclusivas que garantirão que a resposta de pesquisa seja disparada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.search.answerKeyword"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.answerKeyword",
  "keywords": [
    "String"
  ],
  "reservedKeywords": [
    "String"
  ],
  "matchSimilarKeywords": "Boolean"
}
```

