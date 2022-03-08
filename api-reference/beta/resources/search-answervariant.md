---
title: Tipo de recurso answerVariant
description: Uma variante de resposta pode ser usada para alterar determinadas propriedades de uma resposta de pesquisa com base no país ou na plataforma.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 99d196273ae772091f236b18d2821288f63eefe9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338118"
---
# <a name="answervariant-resource-type"></a>Tipo de recurso answerVariant

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma variante de resposta pode ser usada para alterar determinados campos de uma resposta de pesquisa com base no país ou na plataforma.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição da variação de resposta mostrada na página de resultados da pesquisa.|
|displayName|String|Nome da variação de resposta exibido nos resultados da pesquisa.|
|webUrl|String|Link de URL de variação de resposta. Quando os usuários clicarem nessa variação de resposta nos resultados da pesquisa, eles irão para essa URL.|
|languageTags|Coleção de cadeias de caracteres|Lista de países ou regiões capazes de exibir essa resposta de pesquisa.|
|plataformas|Coleção microsoft.graph.platform|Lista de dispositivos e sistemas operacionais capazes de exibir essa variação de resposta. Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.search.answerVariant"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.answerVariant",
  "displayName": "String",
  "webUrl": "String",
  "description": "String",
  "languageTags": ["String"],
  "platforms": ["String"]
}
```

