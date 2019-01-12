---
title: tipo de recurso de embeddedSIMActivationCode
description: O código de ativação SIM incorporado como fornecido pela operadora móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af8bf020953dbc014f42aa6d363d3ca9e30db8a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987402"
---
# <a name="embeddedsimactivationcode-resource-type"></a>tipo de recurso de embeddedSIMActivationCode

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O código de ativação SIM incorporado como fornecido pela operadora móvel.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|O identificador de cartão de circuito integrado (ICCID) para que isso incorporada código de ativação SIM conforme fornecido pela operadora móvel.
A entrada deve coincidir com a seguinte expressão regular: ' ^\[0-9\]{19}\[0-9\]?$ '.|
|matchingIdentifier|String|MatchingIdentifier (MatchingID) conforme especificado na GSMA associação SGP.22 RSP especificação técnica da seção 4.1.
A entrada deve coincidir com a seguinte expressão regular: ' ^\[a-zA-Z0-9\-\]* $'.|
|smdpPlusServerAddress|String|O nome de domínio totalmente qualificado da SM-DP + servidor conforme especificado na especificação técnica RSP GSM associação SPG.22.
A entrada deve coincidir com a seguinte expressão regular: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) *\.) +\[a-zA-Z\]{2,}$'.|

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





