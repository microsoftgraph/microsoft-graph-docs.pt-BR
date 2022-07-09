---
title: Tipo de recurso accessReviewQueryScope
description: Define o que será revisado em uma revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6fb31d3b040177e1065355bab7756b5bdf20ae02
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697866"
---
# <a name="accessreviewqueryscope-resource-type"></a>Tipo de recurso accessReviewQueryScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Um objeto accessReviewQueryScope define o que será revisado em uma revisão [de acesso](../resources/accessreviewsv2-overview.md). Para definir o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

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
