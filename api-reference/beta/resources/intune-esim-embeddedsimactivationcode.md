---
title: tipo de recurso embeddedSIMActivationCode
description: O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c44b685c46b300ced8d81d61de9308648c69eacc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787628"
---
# <a name="embeddedsimactivationcode-resource-type"></a>tipo de recurso embeddedSIMActivationCode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|integratedCircuitCardIdentifier|Cadeia de caracteres|O ICCID (identificador de cartão de circuito integrado) para este código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.
a entrada deve corresponder à seguinte expressão regular: ' ^\[0-9\]{19}\[0-9\]? $ '.|
|matchingIdentifier|Cadeia de caracteres|O MatchingIdentifier (matchid) conforme especificado na SGP de associação GSMA. 22 RSP Technical Specification seção 4,1.
A entrada deve corresponder à seguinte expressão regular: ' ^\[a-zA-Z0-9\-\]* $ '.|
|smdpPlusServerAddress|Cadeia de caracteres|O nome de domínio totalmente qualificado do servidor SM-DP + conforme especificado na especificação técnica SPG da Associação GSM .22 RSP.
A entrada deve corresponder à seguinte expressão regular: ' ^ (\[a-zA-Z0-9\]+ (-\[a-zA-Z0-9\]+) *\.) +\[a-zA-Z\]{2,}$ '.|

## <a name="relationships"></a>Relações
Nenhuma

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





