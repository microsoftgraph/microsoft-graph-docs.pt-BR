---
title: Tipo de recurso recommendedAction
description: Representa ações recomendadas para um locatário com base na simulação de ataque e na campanha de treinamento para melhorar sua postura de segurança.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8932b20e38da6f544f9f9e668b8b304f49fbde6c
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979453"
---
# <a name="recommendedaction-resource-type"></a>Tipo de recurso recommendedAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa ações recomendadas para um locatário com base na simulação de ataque e na campanha de treinamento para melhorar sua postura de segurança.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionWebUrl|String|URL da Web para a ação recomendada.|
|potentialScoreImpact|Duplo|Melhoria potencial na pontuação de segurança do locatário a partir da ação recomendada.|
|title|Cadeia de caracteres|Título da ação recomendada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recommendedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recommendedAction",
  "actionWebUrl": "String",
  "title": "String",
  "potentialScoreImpact": "Double"
}
```

