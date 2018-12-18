---
title: tipo de recurso de embeddedSIMActivationCode
description: O código de ativação SIM incorporado como fornecido pela operadora móvel.
author: tfitzmac
ms.openlocfilehash: 4e768a4047b8ddc785b545d3b850128a8e44f256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311785"
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





