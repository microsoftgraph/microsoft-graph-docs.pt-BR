---
title: Tipo de recurso accessReviewQueryScope
description: Define o que precisa ser revisado em uma revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84c89344ffbb043ee839b2c228a691c2c47e7c32
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696501"
---
# <a name="accessreviewqueryscope-resource-type"></a>Tipo de recurso accessReviewQueryScope

Namespace: microsoft.graph

Um objeto accessReviewQueryScope define o que é revisado em uma revisão [de acesso](../resources/accessreviewsv2-overview.md). Para definir o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|consulta|Cadeia de caracteres|A consulta que representa o que será revisado em uma revisão de acesso.|
|queryRoot|Cadeia de caracteres|No cenário em que os revisores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a origem relativa da consulta. Essa propriedade só será necessária se uma consulta relativa for especificada. Por exemplo, `./manager`.|
|queryType|Cadeia de Caracteres|Indica o tipo de consulta. Os tipos incluem `MicrosoftGraph` e `ARM`.|

É altamente recomendável **especificar a propriedade @odata.type** com o `#microsoft.graph.accessReviewQueryScope` valor. Para obter mais informações sobre as  opções de configuração para escopo usando **accessReviewQueryScope**, consulte Configurar o escopo de sua definição de revisão de acesso usando o [Microsoft API do Graph](/graph/accessreviews-scope-concept).

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
