---
title: Tipo de recurso accessReviewQueryScope
description: Define o que precisa ser revisado em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cc6a8453b804e33eff2788b280928219ddf191cec4f49d2cb1b8c76725eab7c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180905"
---
# <a name="accessreviewqueryscope-resource-type"></a>Tipo de recurso accessReviewQueryScope

Namespace: microsoft.graph

Um objeto accessReviewQueryScope define o que é revisado em uma revisão [de acesso.](../resources/accessreviewsv2-root.md) Para analisar o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|consulta|Cadeia de caracteres|A consulta que representa o que será revisado em uma revisão de acesso.|
|queryRoot|Cadeia de caracteres|No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa for especificada. Por exemplo, `./manager`.|
|queryType|Cadeia de caracteres|Indica o tipo de consulta. Os tipos `MicrosoftGraph` incluem `ARM` e .|

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
