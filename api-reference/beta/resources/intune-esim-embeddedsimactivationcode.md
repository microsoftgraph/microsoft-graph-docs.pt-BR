---
title: tipo de recurso embeddedSIMActivationCode
description: O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28a2344c6e31e944074bc14a7c779a3f165e506a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469108"
---
# <a name="embeddedsimactivationcode-resource-type"></a>tipo de recurso embeddedSIMActivationCode

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|O ICCID (identificador de cartão de circuito integrado) para este código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.
A entrada deve corresponder à seguinte expressão regular: ' ^\[0-9\]{19}\[0-9\]? $ '.|
|matchingIdentifier|String|O MatchingIdentifier (matchid) conforme especificado na SGP de associação GSMA. 22 RSP Technical Specification seção 4,1.
A entrada deve corresponder à seguinte expressão regular: ' ^\[a-zA-Z0-9\-\]* $ '.|
|smdpPlusServerAddress|String|O nome de domínio totalmente qualificado do servidor SM-DP + conforme especificado na especificação técnica SPG da Associação GSM .22 RSP.
A entrada deve corresponder à seguinte expressão regular: ' ^ (\[a-zA-Z0-9\]+ (-\[a-zA-Z0-9\]+) *\.) +\[a-zA-Z\]{2,}$ '.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```



