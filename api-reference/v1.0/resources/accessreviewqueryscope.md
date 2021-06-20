---
title: Tipo de recurso accessReviewQueryScope
description: Define o que precisa ser revisado em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5217524105fd5dcca0248b331f5cc5d0584784aa
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030977"
---
# <a name="accessreviewqueryscope-resource-type"></a>Tipo de recurso accessReviewQueryScope

Namespace: microsoft.graph

Um objeto accessReviewQueryScope define o que é revisado em uma revisão [de acesso.](../resources/accessreviewsv2-root.md) Para analisar o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|consulta|String|A consulta que representa o que será revisado em uma revisão de acesso.|
|queryRoot|String|No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa for especificada. Por exemplo, `./manager`.|
|queryType|String|Indica o tipo de consulta. Os tipos `MicrosoftGraph` incluem `ARM` e .|

A especificação da **propriedade @odata.type** com o valor `#microsoft.graph.accessReviewQueryScope` é altamente recomendada. Para obter mais  informações sobre opções de configuração para escopo usando **accessReviewQueryScope,** consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).

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
