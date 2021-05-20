---
title: Tipo de recurso accessReviewQueryScope
description: Define o que será revisado em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 07a13d12b821d055c8200da2fa5450958a8f53ee
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579275"
---
# <a name="accessreviewqueryscope-resource-type"></a>Tipo de recurso accessReviewQueryScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Um objeto accessReviewQueryScope define o que será revisado em uma revisão [de acesso.](../resources/accessreviewsv2-root.md) Para analisar o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

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
